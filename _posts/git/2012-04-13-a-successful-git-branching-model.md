---
layout: post
title: git����Э����������
description: git����Э����������
keywords: git
category : git
tags : [git]
---

ʱ��ִ٣��������ޣ���������(����û�о���ʵ����֤�����Կ��ܻ�������)����ӭָ�� :)

����������̾��ǻ���[a successful git model](http://nvie.com/posts/a-successful-git-branching-model/)��ƪ���¶�����

**��Ŀ����**��

    ���� / ���� / ���� ���㹲ͬЭ��������һ�ײ���ϵͳ

**��Ŀ�ֹ�**��

    ���� / ���� ��������ϵͳ
    ���� ��������ϵͳ

## ��������˲ֿ�

git��Ȼ�Ƿֲ�ʽ�汾�����ߣ���Ϊ�˷������������Ҫ����һ�����Ĳֿ⣬���ڷ���˽���������֧

    master
    develop

master�����ȶ���(production ready)��������Աƽʱ�Ĵ��붼�ύ��develop��֧��

## �����ߵ�Git��֧

### ������Git��֧

��Ϊ����������ͬʱ��������ϵͳ�����Ծ���������ķ�֧

    # ������Git��֧
    article (local)
    lisi/article (via git remote add lisi http://lisi-server/lisi.git)
    origin/master (via git remote add origin http://remote-server/blog.git)
    origin/develop

### ���ĵ�Git��֧

���������ƣ�����article server�����������

    # ���ĵ�Git��֧
    article (local)
    zhangsan/article (via git remote add zhangsan http://zhangsan-server/zhangsan.git)
    origin/master (via git remote add origin http://remote-server/blog.git)
    origin/develop

### �����Git��֧

��Ϊֻ������һ���˿�������ϵͳ������ֻҪһ��Զ�̷�֧������

    # �����Git��֧
    comment (local)
    origin/master (via git remote add origin http://remote-server/blog.git)
    origin/develop

## ��������

���������ļ��������������µĹ�����ǰ����ʾ�����ĸ������µķ���ͱ�ǩϵͳ��

����������һ���ֺ�(n�α���`commit`)���ύ�����ص�git server(Ҳ����������ӵ�`http://zhangsan-server/zhangsan.git`)��

���Ŀ�����һ���ֺ���ΪҪ�����������Ĳ��ֺϲ���������Ҫִ��һ��`rebase`��`merge`

    # ��ǰ��article��֧��
    git rebase zhangsan/article# �ύ�����ص�git server (Ҳ����������ӵ�http://lisi-server/lisi.git)��
    git push local/article master

��ʱ�����ֿ�������һ���֣���Ҳ���߸�����һ�������̣�`rebase` & `push` (����г�ͻ�����֮)��

����������ͳһ����ÿ�յĿ��������ύ��remote develop��֧�ϣ�������ִ����������˵�����̺��ύ������˵�develop��֧������ʱ�ܿ��������Ѿ�����д�Ĵ����ύ�ˣ�����Ҫ��ִ��һ��`rebase`

    git rebase origin/develop
    git push origin develop

�������������ĵĴ���Ͷ��ύ���˷���˵�develop��֧�ϡ������Ǳߵ�����Ҳһ����ֻ�����˱���ͬ���Ĺ��̡�

## ������ϣ�������Խ׶�

��������Ŀ������������ܶ��ѻ�����ɣ������Ҫ������Խ׶Ρ������������ڷ���������һ����֧������Ϊrelease��������ʱ����˾���3����֧��

    master
    develop
    release

��λͬѧ���ڱ����½�һ��branch����Ӧ����˵�release��֧

    git checkout -b release origin/release

�ֱ���в��ԣ�����������⣬��ִ��`pull` & `push`

    # ��ǰ��release��֧��
    git pull origin release
    git push origin develop

��������Ĳ��Ժ󣬷���ûʲô�����ˣ��Ϳ��Է����ȶ����ˣ�����Ϊ0.1

    git checkout master
    git rebase origin/release
    git tag 0.1
    git push origin master --tags

ͬʱ�����˰�release��֧�ϵĴ�����develop��֧�ϲ�����֤develop��֧�ϲ�����������bug��(û���ҵ����ֱ��`merge`���������`branch`�ķ���)

    git checkout develop
    git rebase origin/release
    git push origin develop
    # ɾ������˵�release��֧
    git push origin :release

�������Ϳ��Լ�����develop��֧�Ͻ��п����ˡ�

## ���������

����ϵͳ��Ҫ���archives���ܣ�������ܵĿ����ͽ�������������������ʱ���ڷ�����¿�һ����֧������Ϊfeature����ʱ����˵ķ�֧�ͱ��������

    master
    develop
    feature/archive

����Ҳ�ڱ��ؽ���һ��archive��֧��ÿ���ύ������˵�feature/archive��������Git��֧��������(����صķ����Git��ʡȥ)

    master
    archive
    origin/feature/archive

�ȵ����feature�������ˣ������˵�develop��ִ֧��һ��`rebase`��Ȼ�����ύ������˵�develop���������͵�archive���ܾ�����

    git checkout archive
    git rebase origin/feature/archive
    git push origin feature/archive# ���Ҫɾ������˵�feature/archive��֧�Ļ�
    git push origin :feature/archive

�����������̸������һ����������Ϻ��½�release��֧�������������bug�޸����޸���Ϻ�`merge`������˵�master��develop

## �����޸�©��

���ͳ�����һ��xss©������Ҫ�����޸�����ʱ�½�һ��hotfix��֧(���ڱ��ؽ���Ȼ���ύ�������)��Ȼ���©�������޸����޸�����ύ������˵�master��develop

    git checkout master
    git pull origin master
    git checkout -b hotfix
    # ©���޸�...
    # �޸����
    git push origin hotfix
    git checkout master
    git rebase hotfix
    git push origin master
    git push origin develop
