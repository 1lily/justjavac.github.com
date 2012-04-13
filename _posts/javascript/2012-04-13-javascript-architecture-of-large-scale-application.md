---
layout:     post
title:      ����Ӧ�õ�javascript�ܹ�
keywords: javascript, �ܹ�
category : javascript
tags : [javascript, �ܹ�]
---

Ŀǰ�ܶ���վ����û����ȷ��ǰ�˼ܹ�������Ƿ������Ⱦ��ͼҳ�������������������һЩjs�������н�����

���ֻ��ʵ��һЩ�򵥵�Ч����û�нϸ��ӵ��߼�����ô���ִ����Ǻ���ģ�
����������jQuery֮���������js����д���������������������ĸо���

��һ����վҪ�İ棬����������վ�ķ�չ���߼����Խ��Խ���ӣ�����Ϊ�˸��õ��û����飬
jsҪ�е������������ʱ���ά����״���䣬��js�ͻ���Խ��Խӷ�ף�Խ��Խ��ά����

���֮�����ǲ���ģ�黯��̣���ҳ��ֳɶ��ģ�飬ģ��֮�以�������
ͨ������/���ķ�ʽ������ģ��佻�����Ӷ�ʹģ����ģ����Ҳ����˵�Ƴ�һ��ģ�鲻��Ե�ǰҳ�����Ӱ�졣

���ģ��Ļ���������ǰ�˺ͺ�˳���Ա����Ч����ϡ�
ǰ��ֻ�������ݵ���ʾ��ҳ��Ľ���������ʱ�������������ݣ�������Ҫ����˳���
��˳���ԱҲ����רע���ṩ�����ã��ȶ��Ľӿڣ�������Ҫ�������ݵ�չʾ��

yahoo�������Ƶ��ϸ�ز�����ǰ��ģ�黯��̣�����ժ¼���£�

## js�ܹ���4����ɲ���

* ģ��(Modules)
* ɳ��(Sandbox)
* Ӧ��(App Core)
* ���(Base Lib)

## ģ��(һ�н�ģ��)

ģ�������һ����������Ҫ����һЩ������ܱ�֤���ᵽ�����鷳

ģ�������ɳ�������������ô����

ģ�鲻֪��ҳ�浽���������ģ�����ֻ֪��ɳ��

ģ��֮��Ҫ����

### ģ��Ĺ���

* �ܺ��Լ�
    * ֻ�ܵ����Լ��Ļ�ɳ��ķ���
    * ��Ҫ���ʲ������Լ���DOM�ڵ�
    * ��Ҫ���ʷ�����ȫ�ֱ���

* �����룬��ʹ��
    * ����Ҫ���κζ�����Ҫ��ɳ���������

* ��Ҫ����߷ŵõ�������
    * ��Ҫ����ȫ�ֱ���

* ��Ҫ��İ����˵��
    * ��Ҫֱ����������ģ��

## ��ȫɳ��

ɳ��Ҫ��֤�ӿڵ�һ���ԣ�ģ�����ʱһ��Ҫ��

ģ��ֻ֪��ɳ�䣬�����ļܹ���ģ������ǲ����ڵ�

ɳ�����һ������Ա��֪����Щ��ģ����Ե��õ�

### ɳ���ְ��

* һ����
    * �ӿ�һ��Ҫ�ɿ�

* ��ȫ��
    * �����һ������ģ����Է��ʵ�

* ����
    * ��ģ��������͵�ϵͳ

�໨Щʱ�������ɳ��ӿڣ���������·������������Ƴ���Ҳ�����޸����з���

## Ӧ�ú���

Ӧ�ú��ĸ���ģ���Ľ���

Ӧ�ú���֪ͨһ��ģ���ʱ�ó�ʼ������ʱ��ע��

Ӧ�ú��Ĵ������

### Ӧ�ú��ĵ�����

* ����ģ�����������
    * ֪ͨһ��ģ���ʱ�ó�ʼ������ʱ��ע��

* �ڲ�ģ���Ľ���
    * ��ģ�龡���ܽ���

* ������
    * ��⣬�������

* ����չ
    * �κο���չ�Ķ����������ʱ


## �������

����״̬�£�ֻ��Ӧ�ú���֪��ʹ�����ĸ����

### ������������

* �����������
* ���õĹ���
    * ����/���л�XML��JSON�ȵ�
    * �������
    * DOM����
    * Ajax����

* �ṩ�ײ�Ŀ���չ��

## ʵ��

��û��ȫ����������˵����ʵ�֣����ǽ���˲���pureMVC��˼�룬�����ƺ�����Щ��

### ����

* һ��ģ���Ӧҳ���ĳһ����
* ģ���ṩ������Mediator���Ե��õķ���
* һ��Mediator����һ���ض���ģ��
* ģ��ֻ��Mediator���ã�ģ��������֪��Mediator�Ĵ���
* Mediator֮��ͨ������/���ĵķ�ʽ���н���

## demo

**ģ�����(����ʹ����John Resig��simple javascript inheritance)**

    var Module = Class.extend({
            init: function(obj) {
                    this.name = obj.name;
                    this.tpl = obj.tpl ? $(obj.tpl).text() : $('#'+obj.name+'-tpl').text();
                    this.$el = obj.el ? $(obj.el) : $('#'+obj.name);
                    this.data = {};
            },
            getTplData: function(data) {
                    return this.data.tplData;
            },
            renderTpl: function(data) {
                    this.data.tplData = data;
                    //ʹ����Mustacheģ������
                    var html = Mustache.to_html(this.tpl, data);
                    this.$el.html(html);
            }});

**�б�ģ��**

    var List = Module.extend({
            // Module �ṩ������Mediator����
            hl: function($item, lock) {
                    var $lis = this.$el.find('li');
                    $lis.each(function(){
                            $(this).removeClass('hl');
                            if (lock) {
                                    $(this).data('locked', false);
                            }
                            if (!lock && $(this).data('locked')) {
                                    $(this).addClass('hl');
                            }
                    });
                    if (lock)
                            $item.data('locked', true);
                    $item.addClass('hl');
            },
            unhl: function($item) {
                    $item.removeClass('hl');
            }});

ǰ��˵��ģ�����׼���÷�������Mediator���á�

**�б�Mediator**

    var ListMediator = Mediator.extend({
            init: function(){
                    var self = this;
                    // ��ʼ��Module
                    this.module =new List({
                            "name": "list"
                    });
                    // ���¼�
                    self.module.$el.delegate('li', 'click', function(e){
                            e.preventDefault();
                            // ����Module����
                            self.module.hl($(this), true);
                            var index = self.module.$el.find('li').index($(this));
                            // ������Ϣ�����м������¼��ķ�����������
                            // ����Ϊobject�������Ժ���Ӽ�ֵ��
                            $.publish(self.module.name+':click', {
                                    "content": self.module.getTplData().list[index].content
                            });
                    }).delegate('li', 'mouseover', function(e){
                            self.module.hl($(this));
                    }).delegate('li', 'mouseout', function(e){
                            self.module.unhl($(this));
                    });
                    // ��ȡԴ���ݣ�ʹ����$.proxy�������ض���context
                    $.getJSON('data.json', $.proxy(function(data){
                            // ����Module�ķ���
                            this.module.renderTpl(data);
                            // ����������������Ϣ
                            $.publish(self.module.name+':loaded', data);
                    }, this));
            }});

���԰�ģ�������Model��Mediator�����Controller��������ʵ���˸��ھۣ�����ϡ�
ÿһ����Ԫ(ģ��+Mediator)�����Ե���ʹ�ã�Ҳ���Ա��Ƴ�������Ӱ�����мܹ���
