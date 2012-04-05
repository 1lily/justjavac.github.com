---
layout: post
title: ���ⳣ��������HTML5�����÷�
description: ���ⳣ��������HTML5�����÷�
category : html5
tags : [html5]
---

ԭ���������� [�˴�](http://html5doctor.com/avoiding-common-html5-mistakes/)��
����Ϊ[Richard Clark](http://html5doctor.com/author/richc/).

����Ϊԭ�����룬ͬʱ��ԭ������һЩ�򻯴���
������ѭ [����-����ҵ��ʹ��Э��](http://creativecommons.org/licenses/by-nc/2.5/cn/)��

## һ����Ҫʹ��section��Ϊdiv�����Ʒ

�����ڱ�ǩʹ����������Ĵ���֮һ�������⽫HTML5��`<section>`�ȼ���`<div>`���������˵��
����ֱ���������Ʒ(������ʽ)��

��XHTML����HTML4�У����ǳ����������Ĵ��룺

    <!-- HTML 4-style code -->
    <div id="wrapper">
      <div id="header">
        <h1>My super duper page</h1>
        <!-- Header content -->
      </div>
      <div id="main">
        <!-- Page content -->
      </div>
      <div id="secondary">
        <!-- Secondary content -->
      </div>
      <div id="footer">
        <!-- Footer content -->
      </div>
    </div>
    
��������HTML5�У�����������

    <!-- �벻Ҫ������Щ���룡���Ǵ���ģ� -->
    <section id="wrapper">
      <header>
        <h1>My super duper page</h1>
        <!-- Header content -->
      </header>
      <section id="main">
        <!-- Page content -->
      </section>
      <section id="secondary">
        <!-- Secondary content -->
      </section>
      <footer>
        <!-- Footer content -->
      </footer>
    </section>
    
����ʹ�ò�����ȷ��*`<section>`��������ʽ����*��
sectionԪ�ر�ʾ�����������������������ĵ���Ҫ�����岿�֡���Ӧ�ð���һ��ͷ����
���������һ������ҳ��������Ԫ��(����HTML����XHTML�ķ��)����ô������Kroc Camen��˵��
ֱ�Ӱ���ʽд��bodyԪ���ϰɡ�
�������Ȼ��Ҫ�������ʽ���������Ǽ���ʹ��div�ɡ�

��������˼�룬���������ȷ��ʹ��HTML5��һЩARIA roles���Ե����ӣ�ע�⣬
�������Լ�����ƣ���Ҳ������Ҫ����div��

    <body>
      <header>
        <h1>My super duper page</h1>
        <!-- Header content -->
      </header>
      <div role="main">
        <!-- Page content -->
      </div>
      <aside role="complementary">
        <!-- Secondary content -->
      </aside>
      <footer>
        <!-- Footer content -->
      </footer>
    </body>
    
����㻹���޷�ȷ��ʹ������Ԫ�أ���ô�ҽ�����ο�[HTML5 sectioning content element flowchart](http://html5doctor.com/flowchart)

## ����ֻ����Ҫ��ʱ��ʹ��header��hgroup

д����Ҫд�ı�ǩ��Ȼ�Ǻ�������ġ�
���ҵ��ǣ��Ҿ�������header��hgroup������������á�
������Ķ�һ�¹���header��hgroupԪ�ص���ƪ������һ����ϸ���˽⣬
���������Ҽ��ܽ����£�

*   headerԪ�ر�ʾ����һ������Ի��ߵ������ʵĸ������֣���������section��ͷ��
*   ��ͷ���ж��ṹʱ����������ͷ���������⣬���ֱ�ʶ���ֵȣ�
    ʹ��hgroup��h1-h6Ԫ�����������Ϊsection��ͷ��

### header������

����header������һ���ĵ���ʹ�ö�Σ�����ʹ�������������ܵ���ӭ��

    <!-- �벻Ҫ������δ��룡�˴�������Ҫheader -->
    <article>
      <header>
        <h1>My best blog post</h1>
      </header>
      <!-- Article content -->
    </article>

������headerԪ��ֻ����һ��ͷ��Ԫ�أ���ô����headerԪ�ذɡ�
��ȻarticleԪ���Ѿ���֤��ͷ����������ĵ���Ҫ�У���header�ֲ��ܰ������Ԫ�أ�������������ģ���
��ôΪʲôҪд����Ĵ��롣�򵥵�д�����������ˣ�

    <article>
      <h1>My best blog post</h1>
      <!-- Article content -->
    </article>
    
### `<hgroup>`�Ĵ���ʹ��

��headers��������ϣ���Ҳ��������hgroup�Ĵ���ʹ�á�
��ʱ��Ӧ��ͬʱʹ��hgroup��header:

* ���ֻ��һ����ͷ��
* ���hgroup�Լ����ܹ����ĺܺá������ⲻ�ϻ�ô

��һ������һ���������ģ�

    <!-- �벻Ҫ������δ���!�˴�����Ҫhgroup -->
    <header>
      <hgroup>
        <h1>My best blog post</h1>
      </hgroup>
      <p>by Rich Clark</p>
    </header>

�����У�ֱ���õ�hgroup����heading�����ɡ�

    <header>
      <h1>My best blog post</h1>
      <p>by Rich Clark</p>
    </header>

�ڶ�����������һ������Ҫ�����ӣ�

    <!-- �벻Ҫ������δ���!�˴�����Ҫheader -->
    <header>
      <hgroup>
        <h1>My company</h1>
        <h2>Established 1893</h2>
      </hgroup>
    </header>

���headerΨһ����Ԫ����hgroup���ǻ�Ҫheader������
���header��û��������Ԫ�أ�������hgroup��������ֱ���õ�header��

    <hgroup>
      <h1>My company</h1>
      <h2>Established 1893</h2>
    </hgroup>

## ������Ҫ�������б�ʽ�����ӷ���nav��

����HTML5������30����Ԫ�أ���ֹ��ԭ�ķ���ʱ���������ڹ������廯�ͽṹ���ı�ǩʱ��ѡ��Ҳ�����Щ�����ء�
Ҳ����˵�����ǲ�Ӧ�����ó����廯��Ԫ�ء�
���ҵ��ǣ�nav��������һ�������õ����ӡ�

navԪ�صĹ淶�������£�

    navԪ�ر�ʾҳ�������ӵ�����ҳ����߱�ҳ���������ֵ����飻�����������ӵ����顣

    ע�⣺��������ҳ���ϵ����Ӷ���Ҫ����navԪ���С������Ԫ�ر�����������Ҫ�ĵ������顣
    �ٸ���������ӣ���footer�о��������ڶ�����ӣ� ����� �������ҳ����Ȩ����ҳ�ȵȡ�
    footerԪ�������Ѿ�����Ӧ����Щ�������ȻnavԪ��Ҳ�������������ͨ��������Ϊ�ǲ���Ҫ�ġ�

    [WHATWG HTML spec](http://www.whatwg.org/specs/web-apps/current-work/complete/sections.html#the-nav-element)

�ؼ��Ĵ����ǡ���Ҫ��"��������Ȼ���ǿ��Ի�������һ����ʲô��������Ҫ��"�����Ҹ�������������ģ�

* ��Ҫ�ĵ���
* վ������
* �����������������飩
* ҳ���ڵ���������ܳ������£�

��Ȼ��û�о��ԵĶԴ����Ը���һ������ʽͶƱ�Լ����Լ��Ľ��ͣ����µ������������Ų��ţ��ҷ���������`<nav>`�У�

* ��ҳ����
* �罻���ӣ���Ȼ��Щ�罻����Ҳ����Ҫ���������硰����"���ղ�"��
* �������µı�ǩ
* �������µķ���
* ��������
* ������footer

����㲻ȷ���Ƿ�Ҫ��һϵ�е����ӷ���nav�У������Լ�����������Ҫ�ĵ�����"
Ϊ�˰�����ش�������⣬����������Ҫԭ��

* ���ʹ��section��hxҲͬ�����ʣ���ô��Ҫ��nav �� [Hixie on IRC](http://krijnhoetmer.nl/irc-logs/whatwg/20091209#l-480)
* Ϊ�˷�����ʣ������ĳ���������ת"�и����nav��ǩ��һ��������

�����Щ����Ĵ��ǡ���"���Ǿ͸�`<nav>`�ϸ�����Ȼ������뿪�ɡ�

## �ġ�figureԪ�صĳ�������

figure�Լ�figcaption����ȷʹ�ã�ȷʵ�����Լ�Ԧ��
������������һЩ�����Ĵ���
�������е�ͼƬ����figure�����У��������߸�λ��Ҫд����Ҫ�Ĵ��롣
�������Ҳ��ͬ���ĵ����ҿ����ܶ���վ�����е�ͼƬ��д��figure��
����ͼƬ�ķ����벻Ҫ�����Ӷ���ı�ǩ�ˡ�
��ֻ�������Լ����ۣ���������ʹ���ҳ�����ݸ�������

�淶�н�figure����Ϊ��һЩ���������ݣ���ʱ����а���������ı���˵����һ�����ĵ����л���Ϊ�����ĵ�Ԫ���á�"
������figure������֮�����������Դ�������ҳ�ƶ���sidebar�У�����Ӱ���ĵ�����

��Щ����Ҳ������֮ǰ�ᵽ��[HTML5 element flowchart](http://html5doctor.com/flowchart)�С�

�������ֻ��Ϊ�˳��ֵ�ͼ��Ҳ�����ĵ������ط����ã��Ǿ;��Բ���`<figure>`��
�����������������һ��ʼ�������Լ��������ͼƬ�Ƿ������������йأ�"
������ǣ��ǿ���Ҳ����<figure>��Ҳ���Ǹ�<aside>����
���������ҿ��԰����ƶ�����¼����"
����������ⶼ���ϣ����������� `<figure>`��

### Logo������figure

��һ����˵��logoҲ��������figure��
�������ҳ�����һЩ����Ƭ�Σ�

    <!-- �벻Ҫ������δ���!���Ǵ�� -->
    <header>
      <h1>
        <figure>
          <img src="/img/mylogo.png" alt="My company" />
        </figure>
        My company name
      </h1>
    </header>

    <!-- �벻Ҫ������δ���!��Ҳ�Ǵ�� -->
    <header>
      <figure>
        <img src="/img/mylogo.png" alt="My company" />
      </figure>
    </header>

ûʲô��˵���ˡ�����Ǻ���ͨ�Ĵ���
���ǿ���Ϊlogo�Ƿ�Ӧ����H1��ǩ�������絽ţ������ؼ��ˣ������ﲻ���������۵Ľ��㡣
�������������� figureԪ�ص����á�
figureֻӦ�ñ��������ĵ��У����߱�sectionԪ��Χ�ơ�

�������logo����̫�����������ķ�ʽ���ðɡ�
�ܼ򵥣��� ��ʹ��figure����ֻ��Ҫ������:

    <header>
      <h1>My company name</h1>
      <!-- More stuff in here -->
    </header>

### FigureҲ������ֻ��ͼƬ

��һ�������Ĺ���figure���������ֻ��ͼƬʹ�á�
figure��������Ƶ����Ƶ��ͼ��һ���������֣����һ�δ��룬һ��ɢ�ģ��Լ��κ����ǻ�����������ϡ�
��Ҫ��figure������ͼƬ��
web��׼��ְ���Ǿ�ȷ���ñ�ǩ�������ݡ�

## �塢��Ҫʹ�ò���Ҫ��type����

���Ǹ����������⣬��������һ����������Ϊ����Ӧ��ͨ�����ʵ�����������ַ��

��HTML5�У�script��styleԪ�ز�����Ҫtype���ԡ�
Ȼ����Щ�ܿ��ܻᱻ���CMS�Զ����ϣ�����Ҫ�Ƴ�Ҳ������ô�����ɡ�
����� �����ֹ������������ȫ���Կ������ģ��Ļ��������û��ʲô������ȥ����type���ԡ�
���е����������Ϊ�ű���javascript����ʽ��css�� ʽ����û��Ҫ�ٶ��һ���ˡ�

    <!-- �벻Ҫ������δ���!��̫������! -->
    <link type="text/css" rel="stylesheet" href="css/styles.css" />
    <script type="text/javascript" src="js/scripts" /></script>

��ʵֻ��Ҫ����д��

    <link rel="stylesheet" href="css/styles.css" />
    <script src="js/scripts" /></script>

����ָ���ַ����Ĵ��붼����ʡ�Ե���
Mark Pilgrim��[Dive into HTML5](http://diveintohtml5.org/semantics.html)�����廯һ���������˽��͡�

## ����form���ԵĴ���ʹ��

HTML5������һЩform�������ԣ�������һЩʹ���ϵ�ע�����

### ��������

һЩ��ý��Ԫ�غ�����Ԫ��Ҳ���в������ԡ�
������˵�Ĺ���Ҳͬ�����á�

��һЩ�µ�form�����ǲ����͵ģ���ζ������ֻҪ�����ڱ�ǩ�У��ͱ�֤����Ӧ����Ϊ�Ѿ����á�

��Щ���԰�����

* `autofocus`
* `autocomplete`
* `required`

̹�׵�˵���Һ��ٿ��������ġ�
��requiredΪ�������������������֣�

    <!-- �벻Ҫ������δ���! ���Ǵ��! -->
    <input type="email" name="email" required="true" />
    <!-- ��һ����������� -->
    <input type="email" name="email" required="1" />

�ϸ���˵���Ⲣû�д󰭡�
�������HTML������ֻҪ����required���Գ����ڱ�ǩ�У���ô���Ĺ��ܾͻᱻӦ�á�
��������㷴����д`equired="false"`�أ�

    <!-- �벻Ҫ������δ���! ���Ǵ��! -->
    <input type="email" name="email" required="false" />

��������Ȼ�Ὣ`required`������Ϊ��Ч��ִ����Ӧ����Ϊ�����������Ÿ�������Ҫȥִ���ˡ�
����Ȼ��������Ҫ�ġ�

��������Ч�ķ�ʽȥʹ�ò������ԡ���������ֻ��xthml����Ч��

* `required`
* `required=""`
* `required="required"`

�������ӵ���ȷд��Ӧ����:

    <input type="email" name="email" required />

