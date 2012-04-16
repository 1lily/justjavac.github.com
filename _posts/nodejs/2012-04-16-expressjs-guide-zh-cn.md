---
layout: post
title: Express.js ��������ָ���ֲ�
tagline: 
description: Express.js ��������ָ���ֲ�
keywords: node.js,javascript, expressjs
category : nodejs
tags : [nodejs, javascript, express.js]
---

[Express](http://expressjs.com/) �ǻ��� [Node.js](http://justjavac.com/nodejs/2012/04/03/node-beginner/)�������ܡ�һ����web������ܡ�

## express �İ�װ

    $ npm install express
    
����

    $ npm install -g express

## ����������

Ҫ���� express.HTTPServer ��ʵ����ֻ��򵥵ĵ��� `createServer()` �������ɡ�ͨ�� HTTPServer ʵ�� app ���ǿ��Զ������ HTTP ������HTTP verbs����·�ɣ�routes����������Ϊ `app.get()`��

    var app = require('express').createServer();

    app.get('/', function(req, res){
      res.send('hello world from justjavac.com!');
    });

    app.listen(3000);

## ���� HTTPS ������

Ҫ��ʼ��һ��express.HTTPSServerʵ�������������ƣ���ͬ������createServer�������Ǵ���һ��������Ϊ���ò������ö������ key�� cert ��������NodeJS https�ĵ����ᵽ�����ò�����

    var app = require('express').createServer({ key: ... });

## ����

Express֧�ֶ๤���������������������Ϳ��������ȡ������߿���ʹ�� `configure()` �������ݵ�ǰ��������Ҫ�������ã�
��configure()û�д��뻷������ʱ�������ڸ�����֮ǰ�����ã�ע���൱�ڱ�������ȷ������������

�����ʾ������ֻ�׳��쳣��dumpException���������ڿ���ģʽ���쳣��ջ�����������Ӧ��
���ǲ��۶Կ������������������Ƕ�ʹ����methodOverride��bodyParser��

�ر�ע���app.router��ʹ�ã������Ա���������Ӧ�õ�·�ɣ���ѡ����
�����״ζ�app.get()��app.post()�ȵĵ��û�����·�ɡ�

    // ���干����
    app.configure(function(){
        app.use(express.methodOverride());
        app.use(express.bodyParser());
        app.use(app.router);
    });

    // ���忪������
    app.configure('development', function(){
        app.use(express.static(__dirname + '/public'));
        app.use(express.errorHandler({ dumpExceptions: true, showStack: true }));
    });

    // ������������
    app.configure('production', function(){
        var oneYear = 31557600000;
        app.use(express.static(__dirname + '/public', { maxAge: oneYear }));
        app.use(express.errorHandler());
    });

�����ڲ��Ͷ������ã�internal��arbitrary����Express�ṩ�� set(key[, val]), enable(key), disable(key)�ȷ�����

    app.configure(function(){
       app.set('views', __dirname + '/views');
       app.set('views');
       // => "/absolute/path/to/views"

       app.enable('some feature');
       // �� app.set('some feature', true); ��ͬ

       app.disable('some feature');
       // �� app.set('some feature', false); ��ͬ

       app.enabled('some feature')
       // => false
    });

Ҫ�޸Ļ���������ͨ������NODE_ENV����������ʵ�֣����磺

    $ NODE_ENV=production node app.js

�����Ҫ����Ϊ���Ļ������ֻ�������������Ż����á�

## ����

Express ֧�����������

* homeΪres.redirect()�ṩӦ�õĻ�׼·����͸���Ĵ����Ѱ�װ��Ӧ�á�
* views��ͼ��views����ĸ�Ŀ¼��Ĭ��ָ��CWD/views
* view engineĬ�ϵ���ͼ��view����������֣���������չ����
* view options��������ȫ����ͼѡ��Ķ���

## ·��

Express����HTTP�����ṩ�������岢���б�������URLӳ��API��
�������ǿ��������û��ʺŵ�URL��������/user/12�����ӣ���������Ӿ���ʵ��������·�ɣ�
������ռλ��ʶ��������Ϊ:id����ص�ֵ���Ա�req.params��ȡ����

    app.get('/user/:id', function(req, res){
        res.send('user ' + req.params.id);
    });

�����е����Ƿ���/user/12ʱ���ء�user 12��,
ע��app.get�൱���ڷ�����ע����һ������get�����¼������������������URL�����һ������ʱ��
ִ�к���Ļص��������ù������첽�ġ�

·����һ�����Ա��ڲ������������ʽ�ļ��ַ��������統/user/:id������󣬱��ڲ�������������ʽ�ַ���������������������ӣ��򻯺󣩣�

    /user/([^/]+)/?

Ҫʵ�ָ��ӵ�ģ����ǿ��Դ���������ʽֱ��������Ϊ���򲶻�����������������ǿ���ͨ��req.params���з��ʣ�
��һ��������Ӧ����req.params[0]���ڶ���Ӧ����req.params[1]���Դ����ơ�

    app.get(/^/users?(?:/(d+)(?:..(d+))?)?/, function(req, res){
        res.send(req.params);
    });

ͨ��Linux��curl�������������Ƕ����·�ɣ�

    $ curl http://justjavac.com:3000/user
    [null,null]
    $ curl http://justjavac.com:3000/users
    [null,null]
    $ curl http://justjavac.com:3000/users/1
    ["1",null]
    $ curl http://justjavac.com:3000/users/1..15
    ["1","15"]

������һЩ·�����ӣ��Լ���֮��ƥ��Ĺ���·����

    "/user/:id"
    /user/12

    "/users/:id?"
    /users/5
    /users

    "/files/*"
    /files/jquery.js
    /files/javascripts/jquery.js

    "/file/*.*"
    /files/jquery.js
    /files/javascripts/jquery.js

    "/user/:id/:operation?"
    /user/1
    /user/1/edit

    "/products.:format"
    /products.json
    /products.xml

    "/products.:format?"
    /products.json
    /products.xml
    /products

    "/user/:id.:format?"
    /user/12
    /user/12.json

���⣬���ǿ���ͨ��POST��ʽ�ύjson���ݣ�Ȼ������bodyParser�м������json�����岢��json���ݷ��ظ��ͻ��ˣ�

    var express = require('express')
      , app = express.createServer();

    app.use(express.bodyParser());

    app.post('/', function(req, res){
      res.send(req.body);
    });

    app.listen(3000);

ͨ��������ʹ�õ�ռλ��������/user/:id����û���κ����ƣ����û����Դ�����ָ����������͵�idֵ��
�������ϣ�������û�idΪ���֣���������д��/user/:id(d+)����
�������ܱ�ֻ֤�и�ռλ����������Ϊ��ֵ���ͲŻ����·�ɵ���ش���

## ·�ɿ���

һ��Ӧ���п��Զ�����·�ɣ����ǿ��Կ���������ת����һ��·�ɣ�Express�ṩ�˵����������� `next()` ������

��һ��ģʽ����ƥ��ʱ�����ƽ���ת��Connect��Express����Connectģ�飩��ͬʱ�м����������������� `use()` �����ӵ�˳����ִ�С�

����������·�ɶ�����ƥ��ͬһ��URLʱҲ����ˣ�����ĳ��·�ɲ������� `next()` ���ѽ���Ӧ������ͻ��ˣ���������Ҳ����˳��ִ�С�

    app.get('/users/:id?', function(req, res, next){
        var id = req.params.id;
        if (id) {
            // ע�����������ͽ���Ӧ����������ͻ��ˣ���ô������URLӳ�佫���ᱻ����
        } else {
            next(); // ������ת����һ������URL��·��
        }
    });

    app.get('/users', function(req, res){
        // do something else
    });

`app.all()` �������Զ�����HTTP����Ӧ�õ�һ������ڣ�������Щ����º����á�

��������ʹ�øù����������ǵ�ģ�����ݿ��м���һ���û��������������req.user��

    var express = require('express')
      , app = express.createServer();

    var users = [{ name: 'www.justjavac.com' }];

    app.all('/user/:id/:op?', function(req, res, next){
      req.user = users[req.params.id];
      if (req.user) {
        next();
      } else {
        next(new Error('cannot find user ' + req.params.id));
      }
    });

    app.get('/user/:id', function(req, res){
      res.send('viewing ' + req.user.name);
    });

    app.get('/user/:id/edit', function(req, res){
      res.send('editing ' + req.user.name);
    });

    app.put('/user/:id', function(req, res){
      res.send('updating ' + req.user.name);
    });

    app.get('*', function(req, res){
      res.send('what???', 404);
    });

    app.listen(3000);

## �м��

�м������ͨ��Connect����express.createServer()���������������ӷ�����һ�������磺

    var express = require('express');

    var app = express.createServer(
        express.logger(),
        express.bodyParser()
    );

���⣬��configure()������������use()���������м����Ҳ��һ�ֺܺõķ�ʽ��

    app.use(express.logger({ format: ':method :uri' }));

ͨ�������м������ͨ��require("connect")�ķ�ʽ���磺

    var connect = require('connect');
    app.use(connect.logger());
    app.use(connect.bodyParser());

�����˸о���Щ��̫ˬ������express��������ˣ�re-exports)��Щ�м�����ԣ�������ʹ���ϱ�����һ���ԣ�

    app.use(express.logger());
    app.use(express.bodyParser());

## ·���м��

����·��ӳ��Ҳ�������Ϊ·�ɵ���˼��·��ͨ������һ���������ӵĻص������������飩�������У��Ӷ����������ض�·�ɵ��м����

�ù��ܶ����Ʒ����Լ�����·��ʹ�õ����ݷǳ����á�

ͨ��������첽���ݵĲ�ѯ����������������ӣ���������ʹ��:id�����������Ի�ȡһ���û���

    app.get('/user/:id', function(req, res, next){
      loadUser(req.params.id, function(err, user){
        if (err) return next(err);
        res.send('Viewing user of justjavac.com ' + user.name);
      });
    });

Ϊ�˱��ִ������ಢ����߿ɶ��ԣ����ǿ������м���ڲ�Ӧ�ø��߼���

�������������ģ����߼������м���������Ǵﵽһ���̶ȵĸ��ã�ͬʱ������ɾ���

    function loadUser(req, res, next) {
      // �����ṩ�����ݣ�����Դ����ݿ��л�ȡ��ʵ�û���Ϣ
      var user = users[req.params.id];
      if (user) {
        req.user = user;
        next();
      } else {
        next(new Error('�����ڵ��û� ' + req.params.id));
      }
    }

    app.get('/user/:id', loadUser, function(req, res){
      res.send('���ڲ鿴�û� ' + req.user.name);
    });

ע���������������·��ӳ��Ļص����������ǿ���֧�ֶ���ġ�

����·���м�����Ա�����˳����ִ�У��Ӷ�����ʵ�ָ����ӵ��߼����������Ʒ���ĳ���û��ķ���Ȩ�ޣ�����Ĵ��뽫ֻ������֤�û��ſ��Ա༭���ʺ���Ϣ��

    function andRestrictToSelf(req, res, next) {
      req.authenticatedUser.id == req.user.id
        ? next()
        : next(new Error('��Ȩ��'));

    }

    app.get('/user/:id/edit', loadUser, andRestrictToSelf, function(req, res){
      res.send('��ʼ�༭�û� ' + req.user.name);
    });

���ס�м���Ǽ򵥵ĺ��������ǻ��ܶ��巵���м���ĺ������Ӷ����Դ���һ�����б������͸����õ����·�����

    function andRestrictTo(role) {
      return function(req, res, next) {
        req.authenticatedUser.role == role
          ? next()
          : next(new Error('��Ȩ��'));

      }
    }

    app.del('/user/:id', loadUser, andRestrictTo('admin'), function(req, res){
      res.send('��ɾ���û� ' + req.user.name);
    });

ע��app.del�ĵ���������֮���Կ�������д������Ϊ�䷵�ص���һ�����������ú������Է��ʡ�admin����ֵ�������漰���հ��ĸ��������������justjavac.com���ұհ�������¡�

ͨ��ʹ�õ��м���ġ�ջ�����Ա���Ϊ���飨�ݹ�Ӧ�ã����룬��˿��Ա���ϲ���ƥ������ӵĹ��ܡ�

    var a = [middleware1, middleware2]
      , b = [middleware3, middleware4]
      , all = [a, b];

    app.get('/foo', a, function(){});
    app.get('/bar', a, function(){});

    app.get('/', a, middleware3, middleware4, function(){});
    app.get('/', a, b, function(){});
    app.get('/', all, function(){});

����ȥexpressԴ��ֿ�鿴������·���м��ʾ����

## HTTP ����

��ǰ��������������Ѿ��Ӵ���app.get()����ˣ�ͬʱExpressҲ�ṩ�˶�����HTTP�����ķ�װ����app.post(), app.del()�ȡ�

����POST��������ӣ����ǵ������ύһ����ʱ������������HTML�н�����method��������Ϊ��post����Ȼ����Ҫ�ڷ���˶���Ըñ��ύ��·�ɿ��ơ�

    <form method="post" action="/">
       <input type="text" name="user[name]" />
       <input type="text" name="user[email]" />
       <input type="submit" value="Submit" />
    </form>

Ĭ�������Express����֪������δ���������壬���������Ҫ����bodyParser�м�������ڷ���application/x-www-form-urlencoded��application/json�����壬���ѱ�������req.body��

���ǿ������������������ʹ�á��м����

    app.use(express.bodyParser());

�����������·�ɾͿ��Է���req.body.user�����ˣ��ö�������ͻ����ύ��name��email���ԡ�

    app.post('/', function(req, res){
      console.log(req.body.user);
      res.redirect('back');
    });

Ҫ�ڱ���ʹ��PUT��HTTP���������ǿ���������Ϊ_method�����ر������ܸı�HTTP������

���ڷ���ˣ�����������Ҫ����methodOverride�м������������bodyParser�м���·����Ӷ��������ð�����ֵ��req.body��

    app.use(express.bodyParser());
    app.use(express.methodOverride());

֮������Ҫ������������Ϊ��Щ����������Ĭ�Ͻ��еģ�ԭ��ܼ򵥣���Ϊ��Щ��Express�����幦����˵�����Ǳ���ģ�����Ӧ�õľ��������㲢��һ����Ҫ��Щ���ܣ�����ͻ���ֱ��֧��PUT��DELETE����Ҳ���Ա�ֱ�ӷ��ʵ���ͬʱmethodOverrideΪ���ṩ��ǿ��Ľ����������������չʾ��PUT��ʹ�ã�

    <form method="post" action="/">
        <input type="hidden" name="_method" value="put" />
        <input type="text" name="user[name]" />
        <input type="text" name="user[email]" />
        <input type="submit" value="Submit" />
    </form>

    app.put('/', function(){
        console.log(req.body.user);
        res.redirect('back');
    });

## ������

Express�ṩ��app.error()����������·�ɻ���next(err)���쳣�������ʾ��Ϊ��ͬ��ҳ���ṩר�ŵ�NotFound�쳣����

    function NotFound(msg){
      this.name = 'NotFound in justjavac.com';
      Error.call(this, msg);
      Error.captureStackTrace(this, arguments.callee);
    }

    NotFound.prototype.__proto__ = Error.prototype;

    app.get('/404', function(req, res){
      throw new NotFound;
    });

    app.get('/500', function(req, res){
      throw new Error('keyboard cat!');
    });

������һ�������ǿ��Զ�ε���app.error()���������Ǽ�������NotFoundʵ������ʾ404ҳ�棬�����䴫����һ��������

ע����Щ������Զ������κεط������ǿ��Է���·�ɿ���listen()֮����

��Ҳ������configure()���������壬�������ǾͿ����Բ�ͬ�Ļ��ڻ����ķ�ʽ�����쳣��

    app.error(function(err, req, res, next){
        if (err instanceof NotFound) {
            res.render('404.jade');
        } else {
            next(err);
        }
    });

�������ʾ���Ǽ������д���Ϊ500���󣬵�����Ը���ϲ��ѡ��

���統node�ڴ����ļ�ϵͳ����ʱ�����п��ܽ��յ������Ĵ��������ENOENT��error.codeΪ��no such file or directory������ʱ���ǿ����ڴ��������н��д���Ȼ����ʾ�ض���ҳ����û���

    app.error(function(err, req, res){
       res.render('500.jade', { error: err });
    });

���ǵ�Ӧ��Ҳ��������Connect errorHandler�м�����㱨�쳣��Ϣ�������������ڡ���������������쳣��stderr��

    app.use(express.errorHandler({ dumpExceptions: true }));

ͬʱ�ڿ����ڼ��������úÿ���HTMLҳ����ʾ�쳣��Ϣʱ����������showStack��ֵΪtrue��

    app.use(express.errorHandler({ showStack: true, dumpExceptions: true }));

�������ͷ `Accept: application/json`��errorHandler�м��Ҳ����json��ʽ������Ӧ��
��������ڿͻ���Javascript��Ӧ�ÿ��������洦��

## ·�ɲ���Ԥ����

·�ɲ���Ԥ����ͨ����ʽ�����ݴ������Դ�����Ӧ�ô���Ŀɶ��Ժ�����URL����֤��

�����㾭���ԵĴӼ���·�ɻ�ȡͨ�����ݣ���ͨ��/user/:id�����û���Ϣ��ͨ�����ǿ��ܻ���������

    app.get('/user/:userId', function(req, res, next){
      User.get(req.params.userId, function(err, user){
        if (err) return next(err);
        res.send('user ' + user.name);
      });
    });

����Ԥ�����������Ա�ӳ�䵽�ص��������Ӷ������ṩ������֤��ǿ���Ըı�ֵ�����������ݿ��м������ݵȹ��ܡ�

�������ǽ�����app.param()����������ϣ��ӳ�䵽ĳ���м���Ĳ��������Կ������ǽ����˰���ռλ����:userId��ֵ��id������

�����������ƽ��һ�������û����ݼ����Լ����������ܼ򵥵�ͨ������next()������Ȩת����һ��Ԥ�����·�ɣ�·�����ƣ���

    app.param('userId', function(req, res, next, id){
      User.get(id, function(err, user){
        if (err) return next(err);
        if (!user) return next(new Error('failed to find user'));
        req.user = user;
        next();
      });
    });

�������������������ᵽ�Ŀ��Դ�����·�ɵĿɶ��ԣ�����������Ӧ���й���ò��ֵ��߼�ʵ�֣��ﵽ����Ŀ�ġ�

    app.get('/user/:userId', function(req, res){
      res.send('justjavac�û�Ϊ ' + req.user.name);
    });

���ڼ򵥵������·��ռλ����֤��ǿ�ȸı�ֵ��ֻ��Ҫ����1��������֧��1�����������ڼ��׳����쳣���Զ�����next(err)��

    app.param('number', function(n){ return parseInt(n, 10); });

Ҳ����ͬʱ���ص�����Ӧ�õ����ռλ��������·��/commits/:from-:to��˵��:from��:to������ֵ���ͣ����ǿ��Խ����Ƕ���Ϊ���飺

    app.param(['from', 'to'], function(n){ return parseInt(n, 10); });

## ��ͼ��Ⱦ

��ͼ���ļ���Ĭ������ѭ `<name>.<engine>` ����ʽ������ `<engine>` ��Ҫ�����ص�ģ������֡�

������ͼlayout.ejs�����ڸ�����ͼϵͳҪrequire("ejs")�������ص�ģ��������exports.compile(str, options)��������Ҫ����һ������������Express��ģ��ӿ�Լ����

����Ҳ����ʹ��app.register()��ӳ��ģ�����浽�����ļ���չ�����Ӷ�ʵ�ָ�����ģ��������Ϊ�����һ���Ϳ���ʵ�֡�justjavac.html�����Ա�ejs��������Ⱦ��

�������ǽ���Jade��������Ⱦindex.html����Ϊ����û������layout:false��index.jade��Ⱦ������ݽ�����Ϊbody���ر�������layout.jade��

    app.get('/', function(req, res){
        res.render('index.jade', { title: 'justjavac, ��עWebǰ�˼�����' });
    });

������view engine���ÿ���ָ��Ĭ��ģ�����棬���������ʹ��jade�����������ã�

    app.set('view engine', 'jade');

�������ǾͿ���ͨ������ķ�ʽ��

    res.render('index');

�������·�ʽ:

    res.render('index.jade');

��view engine���ú�ģ�����չ���ͳ��˿�ѡ�ͬʱ���ǻ����Ի��ƥ���ģ�����棺

    res.render('another-page.ejs');

Expressͬʱ�ṩ����ͼѡ��(view options)���ã���Щ���û���ÿ����ͼ��Ⱦ��Ӧ�ã������㲢������ʹ��layouts���Ϳ����������ã�

    app.set('view options', {
        layout: false
    });

�����Ҫ����Щ���ÿ����ں�����res.render()�����б����ǣ�

res.render('justjavac-view.ejs', { layout: true });

����ͨ��ָ��һ��·���ķ�ʽ��ʵ�����Լ���layout������ϵͳĬ�ϵģ�����������ǽ���view engine������Ϊjade�����Զ�����һ����Ϊ��./views/mylayout.jade����layout�����ǿ�������ʹ������

    res.render('page', { layout: 'mylayout' });

�������ָ����չ����

    res.render('page', { layout: 'mylayout.jade' });

��Щ·��Ҳ�����Ǿ���·����

    res.render('page', { layout: __dirname + '/../../mylayout.jade' });

�ⷽ��Ϻõ����Ӿ����Զ���ejsģ��Ŀ�ʼ�͹رյı�ǣ�

    app.set('view options', {
        open: '{{',
        close: '}}'
    });

## �ֲ���ͼ

Express��ͼϵͳԭ��֧�־ֲ��ͼ�����ͼ�������΢����ͼ����Ҫ������Ⱦһ���ĵ�Ƭ�Ρ�

������������ͼ��ѭ����ʾ���ۣ�����ʹ�þֲ����ϣ�partial collection����

    partial('comment', { collection: comments });

�������Ҫ����ѡ��򱾵ر��������ǿ���ʡ�Զ�����򵥵Ĵ����������飬��������ʾ����һ���ģ�

    partial('comment', comments);

��ʹ�þֲ�����ʱ��֧��һЩ��ħ�������ر�����

    firstInCollection ��Ϊ��һ������ʱ��ֵΪtrue
    indexInCollection �����ж��������ֵ
    lastInCollection ��Ϊ���һ������ʱΪtrue
    collectionLength ���ϵĳ���

���루�����ɣ��ı��ر������ȣ������븸��ͼ�ı��ر���������ͼ����Ч��������������partial(��blog/post��, post)����Ⱦ������־ʱ��������post�ı��ر����������ñ���������ͼӵ�б����û�������blog/post��ͼ��Ȼ��Ч��

������ʾ����ʹ�þֲ�������Ⱦ100���ȵ��������ζ����Ҫ��Ⱦ100����ͼ�����ڼ򵥵ļ�������Խ�ѭ������������Ҫʹ�þֲ����ϣ��������Լ���ϵͳ������


## ��ͼ����

��ͼ����������ڸ���ͼ���еģ�����������һ����Ϊ��views/user/list.jade����ҳ����ͼ������ڸ���ͼ�е���partial(��edit��)����ͼϵͳ���᳢�Բ��Ҳ����ء�views/user/edit.jade������partial(��../messages��)�����ء�views/messages.jade����

��ͼϵͳ��֧������ģ�壬������Ϳ���ʹ��һ��ͬ����Ŀ¼�����磬��һ��·��������ִ��res.render(��users��)���⽫ָ��views/users.jade�����ߡ�views/users/index.jade����

��ʹ�������������ͼʱ�����ǿ���ͨ��partial(��users��)��ͬ��Ŀ¼�����á�views/users/index.jade����ͬʱ��ͼϵͳ�᳢�ԡ�../users/index�������ܼ������ǵ���partial(��index��)����Ҫ��

## ģ������

Express֧�����ģ�����棬���õ��У�

* Haml haml ��ʵ��
* Jade haml.js �����ߣ�ͬʱҲ��Express��Ĭ��ģ������
* EJS Ƕ��JavaScriptģ��
* CoffeeKup ����CoffeeScript��ģ������
* jQuery Templates ��NodeJS�汾

##  Session Support

������Express��ͨ������Connect��session�м��������Session֧�֣���Ȼǰ������Ҫ����֮ǰʹ��cookieParser�м�������ڷ����ʹ���req.cookies��cookie����(����֪��session������cookie����ͨ�ű��ֵ�)��

    app.use(express.cookieParser());
    app.use(express.session({ secret: "keyboard cat" }));

Ĭ��session�м��ʹ��Connect�󶨵��ڴ�洢����Ҳ�������ʵ�ַ�ʽ������connect-redis���ṩ��һ��Redis��session�洢������

    var RedisStore = require('connect-redis');
    app.use(express.cookieParser());
    app.use(express.session({ secret: "justjavac�����ַ���", store: new RedisStore }));

����req.session��req.sessionStore���ԾͿ��Ա�����·�ɼ��¼��м�������ʣ�req.session�����Ի������ÿһ����Ӧ���͸��ͻ��ˣ�������һ�����ﳵ�����ӣ�

    var RedisStore = require('connect-redis');
    app.use(express.bodyParser());
    app.use(express.cookieParser());
    app.use(express.session({ secret: "keyboard cat", store: new RedisStore }));

    app.post('/add-to-cart', function(req, res){
      // ����bodyParser()�м������POST�ύ�ı�����
      var items = req.body.items;
      req.session.items = items;
      res.redirect('back');
    });

    app.get('/add-to-cart', function(req, res){
      // ��ҳ��ص����ز�ͨ��GET����/add-to-cart ʱ
      // ���ǿ��Լ��req.session.items && req.session.items.length��Ȼ����Ϣ��ӡ��ҳ��
      if (req.session.items && req.session.items.length) {
        req.flash('info', 'You have %s items in your cart', req.session.items.length);
      }
      res.render('shopping-cart');
    });

req.session����ӵ�����������������Session#touch(), Session#destroy(), Session#regenerate()������session����������Ϣ��鿴 [Connect Session�ĵ�](http://senchalabs.github.com/connect/middleware-session.html)��