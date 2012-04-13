---
layout: post
title: ��� Web ����Ĭ������
keywords: web, ����, css
category : web
tags : [web, ����]
---

����Ա�����ҳ�и�СС�� Ĭ����������粨������Ĭ������Զ�����������еĸ��ӡ���ǰ��Ҫ��ע font-family ���������� lang ���Ժ� charset ���á��������˸����꾡�Ĳ��ԣ�

<http://lifesinger.github.com/lab/2011/default-fonts/>

�ڲ�ͬ����ϵͳ�£��ø���������򿪣��ر��� Firefox �� Opera�����ҵ����簡��������������������Ȥȫ�ޣ�

��Ȼ��ɥ����ߣ��������о��Ĺ������ǵü�����

* lang, charset �� font-family �����Ĭ���������Ӱ�죬���ɺܸ��ӡ�
* �����ƫ������������ã���Ĭ��������ֱ��Ӱ�죬���� WebKit �ں˵� Chrome �������
* ����ת�� ��\5b8b\4f53�� Ҳ����ͨ������������������� Mac OS �� Chrome �У�ֻ��ʶ simsun.
* <del>������ʵ�� serif �г������壬����� sans-serif, �߼����Ǵ�ġ�</del>
  ����������û�й涨ǰ��� font name Ҫ������ general family ����һ�£�
* ��ͬ����ϵͳ�£����������Ĭ�ϵ� sans-serif �������壬һ�㶼�����ѡ����û��ѵ���Ϊ��ѣ�����ǿ���û��������塣

��Ŀǰ�û�������������������� 12px ��СΪ������ҳ����У�**��ѵ�����Ĭ�����巽���ǣ�Windows �������壬��������ϵͳ�����źڵ��޳�������**��δ�����ŵ�����Ļ�ı��ͷֱ��ʵ���ߣ��������Ĭ�ϴ�С��ߵ� 14px ����ʱ���������в���ϵͳ�£��������Ĭ�������ͳһΪ�źڵ��޳������塣

Ϊ����������ҳ�ھ����ܶ������£������������������Ⱦ����Ҫ�ر������¼��㣺

* �� Mac Chrome �Ȼ����£��� font-family: times, sans-serif ʱ��
  �������岢������� sans-serif ��Ⱦ�����ǻ���� times �� serif ���ԣ�
  ѡ��Ĭ�ϵ� serif ������������Ⱦ��
  ������ Mac Chrome �£�Ĭ�� serif ���������Ǻܽӽ������һ�����壬�Ƚ��ѿ���
  ��������ʵ�������Ϊ���ӣ���ο������е����ۣ�
* �� Firefox �У�ֻҪ font-family �������壬���ı�Ȼ��������չ�֡�
  ���� font-family �в��������塣
* �� lang=��zh-CN��, charset=��utf-8�� ʱ��
  font: arial �� Mac Firefox �Ȼ����£�Ĭ���������������塣
* ��Ӣ�� Win7 �£�ֻҪ charset=��gbk��, �� font-family Ϊ arial, sans-serif ʱ��
  <del>Ĭ�����������Ǻ��ѿ��� Microsoft Sans Serif Regular.</del>
  ���������� fallback ���˺������� Dotum/Gulim��gulim.ttc������ʾ��
  Dotum/Gulim û�е��ַ����ջ� fallback �� SimSun����ʱ��֪�����������Ƿ�����м䡣
  �� Microsoft Sans Serif û��һ���ϵ����
* Opera �Ǹ��ֲ������磬��Ҫ���Է�������ɣ�������һ�¾ͺá�

�����ܽ����

1 ���ҳ�� charset �� utf-8, ������Ĭ�����巽���ǣ�

        font-family: arial, sans-serif;

  ����ʡ�� lang ��������Ϊ zh-CN, �ڸ��ֻ����¶�����Ԥ�ڡ�

2 ���ҳ�� charset �� gbk, �Ƽ�Ĭ�����巽��Ϊ��

        font-family: arial;

  Chrome OS ��δ���ԣ����ݳ³ɲ����ϵķ�����
  �������Ϊû�� sans-serif ����������������ѿ���
  �������� Chrome OS ��δ��ʽ������Ŀǰ�����Ⱥ��ԡ�

��󣬸����Ƽ���������ҳ������ʵ��Ϊ��

    html lang=zh-CN
    charset=utf-8
    font-family: arial, sans-serif;

���Ի���˵����

    Mac OS X 10.6.7
    Chrome 10.0.648.204
    Firefox 4.0
    Safari 5.0.4
    Opera 11.01

    Win7 Ultimate
    IE 9.0.8080.16413

���䣺

1 ���������Ĭ�ϴ�С���иߵ���Ϣ���Ƽ����ģ�[Ĭ�� Web ������ʽ][1]
2 ��������� fallback ���ı���Ⱦ��Ϣ���Ƽ����ģ�[����������Ⱦ�ı�][2]

[1]: http://justjavac.com/web/2012/04/12/default-web-font-style
[2]: http://justjavac.com/web/2012/04/12/how-do-browsers-render-text