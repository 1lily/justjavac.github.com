---
layout: post
title: Node����
description: Node����
keywords: node.js,javascript
category : nodejs
tags : [nodejs, javascript]
---

<h1>Node����</h1>

        <div id="author">���ߣ� <a href="http://twitter.com/manuelkiessling">Manuel Kiessling</a><br />
                         ���룺 <a href="http://weibo.com/goddyzhao">goddyzhao</a> & 
                               <a href="http://www.otakustay.com">GrayZhang</a> & 
                               <a href="http://weibo.com/cmonday">MondayChen</a></div>

        <a name="about"></a>

        <h2>����</h2>

        <p>
            ���������ڽ̻��������Node.js������Ӧ�ã������лᴫ������������ġ��߼���JavaScript֪ʶ�����������һ����Hello World���Ľ̡̳�
        </p>

        <a name="status"></a>

        <h3>״̬</h3>

        <p>
            �������Ķ����Ѿ��Ǳ�������հ档��ˣ�ֻ�е����д�������Լ�����°汾Node.js�ĸĶ����ж�Ӧ������ʱ���Ż���и��¡�
        </p>

        <p>
            �����еĴ��밸������Node.js 0.6.11�汾�в��Թ���������ȷ������
        </p>

        <a name="intended-audience"></a>

        <h3>���߶���</h3>

        <p>
            �������ʺ����������Ƽ��������Ķ��ߣ� ���ٶ�һ������Ruby��Python��PHP����Java������������������һ���ľ��飻��JavaScript���ڳ�ѧ�׶Σ�������ȫ��һ��Node.js�����֡�
        </p>

        <p>
            ����ָ���ʺ϶��������������һ������Ŀ����ߣ���˼��˵�����鲻��������������͡����������ƽṹ�ȵ�֮��ǳ������ĸ��������ܡ�Ҫ�������飬��Щ�����ĸ����Ҷ�Ĭ�����Ѿ����ˡ�
        </p>

        <p>
            Ȼ�������黹�ǻ��JavaScript�еĺ����Ͷ�������ϸ���ܣ���Ϊ����������ͬ���������еĺ����Ͷ����кܴ�Ĳ�ͬ��
        </p>

        <a name="structure"></a>

        <h3>����ṹ</h3>

        <p>
            ���걾��֮���㽫���һ��������webӦ�ã���Ӧ�������û����ҳ���Լ��ϴ��ļ���
        </p>

        <p>
            ��Ȼ�ˣ�Ӧ�ñ���û��ʲô�˲���ģ����Ϊ��ʵ�ָù�����д�Ĵ��뱾�����Ǹ���ע������δ���һ�������������Ӧ�õĲ�ͬģ����иɾ��ذ��롣 �ǲ��Ǻ��������Ժ���������ˡ�
        </p>

        <p>
            �����ȴӽ�����Node.js�����н���JavaScript������������������н���JavaScript�����Ĳ��쿪ʼ��
        </p>

        <p>
            �����ţ�����������һ���ͳ�ġ�Hello World��Ӧ�ã���Ҳ���������Node.jsӦ�á�
        </p>

        <p>
            ��󣬻�ʹ������������һ����������������Ӧ�ã�����Ҫ��ɸ�Ӧ����Ҫʵ�ֵĲ�ͬģ�飬��һ��һ�����������ʵ����Щģ�顣
        </p>

        <p>
            ����ȷ�����ǣ���������У���һ�ѧ��JavaScript��һЩ�߼��ĸ�����ʹ�������Լ�Ϊʲôʹ����Щ����Ϳ���ʵ�ֶ��������������ͬ��ĸ�����޷�ʵ�֡�
        </p>

        <p>
            ��Ӧ�����е�Դ���붼����ͨ��
            <a href="https://github.com/ManuelKiessling/NodeBeginnerBook/tree/master/code/application">����Github����ֿ�</a>.
        </p>

        <div id="table-of-contents-headline">Ŀ¼</div>
        <div id="table-of-contents">
            <ul>

                <li><a href="#about">����</a>
                    <ul>
                        <li><a href="#status">״̬</a></li>
                        <li><a href="#intended-audience">���߶���</a></li>
                        <li><a href="#structure">����ṹ</a></li>
                    </ul>
                </li>

                <li><a href="#javascript-and-nodejs">JavaScript��Node.js</a>
                    <ul>
                        <li><a href="#javascript-and-you">JavaScript����</a></li>
                        <li><a href="#a-word-of-warning">�������</a></li>
                        <li><a href="#server-side-javascript">��������JavaScript</a></li>
                        <li><a href="#hello-world">��Hello World��</a></li>

                    </ul>
                </li>
                <li><a href="#a-full-blown-web-application-with-nodejs">һ�������Ļ���Node.js��webӦ��</a>
                    <ul>
                        <li><a href="#the-use-cases">����</a></li>
                        <li><a href="#the-application-stack">Ӧ�ò�ͬģ�����</a></li>
                    </ul>

                </li>
                <li><a href="#building-the-application-stack">����Ӧ�õ�ģ��</a>
                    <ul>
                        <li><a href="#a-basic-http-server">һ��������HTTP������</a></li>
                        <li><a href="#analyzing-our-http-server">����HTTP������</a></li>
                        <li><a href="#passing-functions-around">���к�������</a></li>
                        <li><a href="#how-function-passing-makes-our-http-server-work">���������������HTTP������������</a></li>

                        <li><a href="#event-driven-callbacks">�����¼������Ļص�</a></li>
                        <li><a href="#how-our-server-handles-requests">����������δ��������</a></li>
                        <li><a href="#finding-a-place-for-our-server-module">����˵�ģ���������</a>
                        </li>
                        <li><a href="#whats-needed-to-route-requests">�������������ġ�·�ɡ�</a></li>
                        <li><a href="#execution-in-the-kongdom-of-verbs">��Ϊ����ִ��</a></li>
                        <li><a href="#routing-to-real-request-handlers">·�ɸ����������������</a></li>

                        <li><a href="#making-the-request-handlers-respond">�����������������Ӧ</a>
                            <ul>
                                <li><a href="#how-to-not-do-it">���õ�ʵ�ַ�ʽ</a></li>
                                <li><a href="#blocking-and-non-blocking">�����������</a></li>
                                <li><a href="#responding-request-handlers-with-non-blocking-operations">�Է�������������������Ӧ</a>
                                </li>
                            </ul>

                        </li>
                        <li><a href="#serving-something-useful">�����õĳ���</a>
                            <ul>
                                <li><a href="#handling-post-requests">����POST����</a></li>
                                <li><a href="#handling-file-uploads">�����ļ��ϴ�</a></li>
                            </ul>
                        </li>

                        <li><a href="#conclusion-and-outlook">�ܽ���չ��</a></li>
                    </ul>
                </li>
            </ul>
        </div>

        <a name="javascript-and-nodejs"></a>

        <h2>JavaScript��Node.js</h2>

        <a name="javascript-and-you"></a>

        <h3>JavaScript����</h3>

        <p>
            �׿����������������������Լ����JavaScript�Ĺ�ϵ�����µ���ҪĿ���������㿴������������Ƿ��б�Ҫ�����Ķ������½ڵ����ݡ�
        </p>

        <p>
            ��������һ������ô�����Ϳ�ʼ����HTML���С���������������ˣ���Ӵ����������JavaScript��Ȥ�Ķ�����������JavaScript����ֻ������Ĳ�������Ϊwebҳ����ӽ�����
        </p>

        <p>
            ����������Ҫ���ǡ��ɻ���������Ҫ֪����ι������ӵ�webվ�� ���� ���ǣ���ѧϰ��һ������PHP��Ruby��Java�����ı�����ԣ�����ʼ��д����ˡ����롣
        </p>

        <p>
            ���ͬʱ���㻹ʼ�չ�ע��JavaScript������ͨ��һЩ��jQuery��Prototype֮�༼���Ľ��ܣ��������˽⵽�˺ܶ�JavaScript�еĽ��׼��ܣ�ͬʱҲ���ܵ���JavaScript���ǽ�����<em>window.open() </em>��ô�򵥡� .
        </p>

        <p>
            ��������Щ�Ͼ�����ǰ�˼��������ܵ���Ҫ��ǿҳ���ʱ��ʹ��jQuery��������ú�ˬ����������㶥���Ǹ�JavaScript<em>�û�</em>������JavaScript<em>������</em>��
        </p>

        <p>
            Ȼ�󣬳�����Node.js������˵�JavaScript�����ж�ᰡ��
        </p>

        <p>
            ���ǣ��������ʱ�������ʰ�����Ϥ��İ����JavaScript�ˡ����Ǳ𼱣�дNode.jsӦ����һ�����飻���Ϊʲô����Ҫ��������д�����ַ�ʽ����д����ζ�š�����Ҫ��JavaScript�������������ˡ�
        </p>

        <p>
            �������ˣ� ����JavaScript���������������֣���������˵��������̬���ڣ���������90�������Ϊ��DHTML������ǿ��С��ߣ�����jQuery�����ϸ������ϵ�ǰ�˼�����һֱ�����ڵķ���˼���������ˣ������ҵ�һ������ȷ���ķ�ʽ��ѧϰJavaScript��ʹ��������дNode.jsӦ�õ�ʱ��о��Լ�������������������������ʹ������
        </p>

        <p>
            ��Ϊ����ǹؼ��� �㱾���Ѿ��Ǹ��о���Ŀ����ߣ��㲻��ͨ������Ѱ�Ҹ��ֽ�����������п��ܻ��в���ȷ�ģ���ѧϰ�µļ�������Ҫȷ���Լ���ͨ����ȷ�ķ�ʽ��ѧϰ�������
        </p>

        <p>
            ��Ȼ�ˣ����治���������ѧϰJavaScript�����¡����ǣ��е�ʱ��⿿��Щ������ԶԶ�����ġ�����Ҫ����ָ����
        </p>

        <p>
            �����Ŀ����Ǹ����ṩָ����
        </p>

        <a name="a-word-of-warning"></a>

        <h3>�������</h3>

        <p>
            ҵ���зǳ������JavaScript����Ա�����Ҳ�������һԱ��
        </p>

        <p>
            �Ҿ�����һ�����������Ǹ��ҡ�����Ϥ��ο������webӦ�ã����Ƕԡ���������JavaScript�Լ�Node.js���Ҷ�ֻ�����֡���Ҳֻ�����ѧϰ��һЩJavaScript�ĸ߼������û��ʵ�����顣
        </p>

        <p>
            ��ˣ����鲢����һ���������ŵ���ͨ�����飬������һ�����ӳ������ŵ��߼����š����顣
        </p>

        <p>
            ����ɹ��Ļ�����ô��������ҵ�����ʼѧϰNode.js��ϣ��ӵ�еĽ̡̳�
        </p>

        <a name="server-side-javascript"></a>

        <h3>�����JavaScript</h3>

        <p>
            JavaScript������������������У�Ȼ�������ֻ���ṩ��һ�������ģ���������ʹ��JavaScript������ʲô������û�С�˵��̫�����JavaScript���Ա��������ʲô����ʵ�ϣ�JavaScript��һ�š������������ԣ� ������ʹ���ڲ�ͬ���������У�������������ͬ����������й�֮���޲�����
        </p>

        <p>
            Node.js��ʵ�Ͼ�������һ�������ģ��������ں�ˣ��������������������JavaScript���롣
        </p>

        <p>
            Ҫʵ���ں�̨����JavaScript���룬������Ҫ�ȱ�����Ȼ����ȷ��ִ�С�Node.js��ԭ��������ˣ���ʹ����Google��V8�������Google��Chrome�����ʹ�õ�JavaScriptִ�л������������ͺ�ִ��JavaScript���롣
        </p>

        <p>
            ����֮�⣬������Node.js�Ļ���������õ�ģ�飬���ǿ��Լ򻯺ܶ��ظ����������������ն�����ַ�����
        </p>

        <p>
            ��ˣ�Node.js��ʵ�ϼ���һ������ʱ������ͬʱ����һ���⡣
        </p>

        <p>
            Ҫʹ��Node.js,������Ҫ���а�װ��������ΰ�װNode.js������Ͳ�׸���ˣ�����ֱ�Ӳο�<a href="https://github.com/joyent/node/wiki/Installation" title="Building and Installing Node.js">�ٷ��İ�װָ��</a>����װ��ɺ󣬼��������Ķ�������������ݡ�
        </p>

        <a name="hello-world"></a>

        <h3>��Hello World��</h3>

        <p>
            ���ˣ����ϻ�������˵�ˣ����Ͽ�ʼ���ǵ�һ��Node.jsӦ�ã���Hello World����
        </p>

        <p>
            ������ϲ���ı༭��������һ��<em>helloworld.js</em>�ļ�������Ҫ��������STDOUT�����Hello World����������ʵ�ָù��ܵĴ��룺
        </p>
        <pre class="prettyprint lang-js"><span class="pln">console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span class="str">"Hello World"</span><span class="pun">);</span></pre>
        
        <p>
            ������ļ�����ͨ��Node.js��ִ�У�
        </p>

        <pre>node helloworld.js</pre>
        <p>
            �����Ļ����ͻ����ն����<em>Hello World</em> ��
        </p>

        <p>
            �ðɣ��ҳ������Ӧ�����е���Ȥ����ô�������Ǿ����㡰�ɻ�����
        </p>


        <a name="a-full-blown-web-application-with-nodejs"></a>

        <h2>һ�������Ļ���Node.js��webӦ��</h2>
 
        <a name="the-use-cases"></a> 
 
        <h3>����</h3> 
 
        <p>��������Ŀ���趨�ü򵥵㣬����ҲҪ��ʵ�ʲ��У�</p>

        <ul>
        <li>�û�����ͨ�������ʹ�����ǵ�Ӧ�á�</li>
        <li>���û�����<em>http://domain/start</em>ʱ�����Կ���һ����ӭҳ�棬ҳ������һ���ļ��ϴ��ı���</li>
        <li>�û�����ѡ��һ��ͼƬ���ύ��������ļ������ϴ���<em>http://domain/upload</em>����ҳ������ϴ�����ͼƬ��ʾ��ҳ���ϡ�</li>
        </ul>

        <p>����ˣ�������Ҳ����ȥGoogleһ�£��ҵ㶫���Ҹ�һ������ɹ��ܡ��������������Ȳ��������</p>

        <p>����һ����˵���������һĿ��Ĺ����У����ǲ�������Ҫ�����Ĵ�������ܴ����Ƿ����š����ǻ�Ҫ�Դ˽��г�����Ѱ��һ���ʺϹ�����Ϊ���ӵ�Node.jsӦ�õķ�ʽ��</p>

        <h3>Ӧ�ò�ͬģ�����</h3>

        <p>�������ֽ�һ�����Ӧ�ã�Ϊ��ʵ�����ĵ�������������Ҫʵ����Щ�����أ�</p>

        <ul>
        <li>������Ҫ�ṩWebҳ�棬�����Ҫһ��<em>HTTP������</em></li>
        <li>���ڲ�ͬ�����󣬸��������URL�����ǵķ�������Ҫ���費ͬ����Ӧ�����������Ҫһ��<em>·��</em>�����ڰ������Ӧ�����������request handler��</li>
        <li>�����󱻷��������ղ�ͨ��·�ɴ���֮����Ҫ���Զ�����д������������Ҫ���յ�<em>���������</em></li>
        <li>·�ɻ�Ӧ���ܴ���POST���ݣ����Ұ����ݷ�װ�ɸ��Ѻõĸ�ʽ���ݸ�����������������Ҫ<em>�������ݴ�����</em></li>
        <li>���ǲ�����Ҫ����URL��Ӧ�����󣬻�Ҫ��������ʾ����������ζ��������ҪһЩ<em>��ͼ�߼�</em>�����������ʹ�ã��Ա㽫���ݷ��͸��û��������</li>
        <li>����û���Ҫ�ϴ�ͼƬ������������Ҫ<em>�ϴ�������</em>�������ⷽ���ϸ��</li>
        </ul>

        <p>�����������룬ʹ��PHP�Ļ����ǻ���ô��������ṹ��һ����˵���ǻ���һ��Apache HTTP������������mod_php5ģ�顣<br />������Ƕȿ�������������HTTP�����ṩWebҳ�桱�������������ҪPHP������</p>

        <p>������Node.js��˵��������ȫ��һ���ˡ�ʹ��Node.jsʱ�����ǲ�������ʵ��һ��Ӧ�ã�ͬʱ��ʵ��������HTTP����������ʵ�ϣ����ǵ�WebӦ���Լ���Ӧ��Web��������������һ���ġ�</p>

        <p>������������һ��ѻ�Ҫ������������ǻ�����ʶ������Node.js��˵�Ⲣ����ʲô�鷳���¡�</p>

        <p>�������Ǿ�����ʼʵ��֮·���ȴӵ�һ������--HTTP���������֡�</p>

        <a name="building-the-application-stack"></a>

        <h2>����Ӧ�õ�ģ��</h2>

        <a name="a-basic-http-server"></a>

        <h3>һ��������HTTP������</h3>

        <p>
            ����׼����ʼд�ҵĵ�һ���������ġ�Node.jsӦ�õ�ʱ���Ҳ�����֪����ôдNode.js���룬Ҳ��֪����ô��֯��Щ���롣
            <br>
            ��Ӧ�ð����ж������Ž�һ���ļ����������кܶ�̶̳����������е��߼����Ž�һ����Node.jsд�Ļ���HTTP����������������������������ݣ�ͬʱ���뱣�ִ���Ŀɶ����أ�
        </p>

        <p>

            ʵ���ϣ�ֻҪ�Ѳ�ͬ���ܵĴ�����벻ͬ��ģ���У����ִ�����뻹���൱�򵥵ġ�
        </p>

        <p>
            ���ַ���������ӵ��һ���ɾ������ļ���main file�����������Node.jsִ������ͬʱ�����ӵ�иɾ���ģ�飬���ǿ��Ա����ļ���������ģ����á�  
        </p>

        <p>
            ��ô����������������һ�������������ǵ�Ӧ�õ����ļ�����һ�����������ǵ�HTTP�����������ģ�顣
        </p>

        <p>

            ���ҵ�ӡ��������ļ�����<em>index.js</em>�������Ǹ���׼��ʽ���ѷ�����ģ��Ž���<em>server.js</em>���ļ�����ܺ���⡣
        </p>

        <p>
            �������ȴӷ�����ģ�鿪ʼ���������Ŀ�ĸ�Ŀ¼�´���һ����<em>server.js</em>���ļ�����д�����´��룺
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br>http</span><span
                class="pun">.</span><span class="pln">createServer</span><span class="pun">(</span><span class="kwd">function</span><span
                class="pun">(</span><span class="pln">request</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; response</span><span class="pun">.</span><span class="pln">write</span><span
                class="pun">(</span><span class="str">"Hello World"</span><span class="pun">);</span><span
                class="pln"><br>&nbsp; response</span><span class="pun">.</span><span class="pln">end</span><span
                class="pun">();</span><span class="pln"><br></span><span class="pun">}).</span><span
                class="pln">listen</span><span class="pun">(</span><span class="lit">8888</span><span
                class="pun">);</span></pre>

        <p>
            �㶨����ո������һ�����Թ�����HTTP��������Ϊ��֤����һ�㣬���������в��Ҳ�����δ��롣���ȣ���Node.jsִ����Ľű���
        </p>
        <pre>node server.js</pre>
        <p>
            �������������������<a href="http://localhost:8888/" rel="nofollow">http://localhost:8888/</a>����ῴ��һ��д�š�Hello World������ҳ�� 
        </p>

        <p>
            �����Ȥ������������������̸̸HTTP�����������⣬�������֯��Ŀ�������ȷ�һ�߰ɣ��������Σ��ұ�֤֮�����ǻ����Ǹ�����ġ�
        </p>

        <a name="analyzing-our-http-server"></a>

        <h3>����HTTP������</h3>

        <p>
            ��ô�������������Ƿ���һ�����HTTP�������Ĺ��ɡ�
        </p>

        <p>
            ��һ��<em>����require��</em>Node.js�Դ��� <em>http</em> ģ�飬���Ұ�����ֵ�� <em>http</em> ������
        </p>


        <p>
            ���������ǵ���httpģ���ṩ�ĺ����� <em>createServer</em> ����������᷵��һ���������������һ������ <em>listen</em> �ķ��������������һ����ֵ������ָ�����HTTP�����������Ķ˿ںš�
        </p>

        <p>
            ������ʱ�Ȳ��� <em>http.createServer</em> ����������Ǹ��������塣
        </p>

        <p>
            ���Ǳ��������������Ĵ���������������������8888�˿ڣ�
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br></span><span class="kwd">var</span><span
                class="pln"> server </span><span class="pun">=</span><span class="pln"> http</span><span
                class="pun">.</span><span class="pln">createServer</span><span class="pun">();</span><span
                class="pln"><br>server</span><span class="pun">.</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span></pre>

        <p>
            ��δ���ֻ������һ������8888�˿ڵķ��������������κα�����飬���������󶼲���Ӧ��
        </p>

        <p>
            ����Ȥ�����ң������֮ǰϰ��ʹ��һ�����ӱ��ص����ԣ�����PHP����������֣��Ĳ����� <em>createSever()</em> �ĵ�һ��������һ���������塣
        </p>

        <p>
            ʵ���ϣ�������������� <em>createServer()</em> �ĵ�һ��Ҳ��Ψһһ����������Ϊ��JavaScript�У���������������һ�����ǿ��Ա����ݵġ�
        </p>

        <a name="passing-functions-around"></a>

        <h3>���к�������</h3>

        <p>
            ������˵���������������
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> say</span><span
                class="pun">(</span><span class="pln">word</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span
                class="pln">word</span><span class="pun">);</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> execute</span><span
                class="pun">(</span><span class="pln">someFunction</span><span class="pun">,</span><span class="pln"> value</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; someFunction</span><span
                class="pun">(</span><span class="pln">value</span><span class="pun">);</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>execute</span><span
                class="pun">(</span><span class="pln">say</span><span class="pun">,</span><span
                class="pln"> </span><span class="str">"Hello"</span><span class="pun">);</span></pre>

        <p>
            ����ϸ�Ķ���δ��룡��������ǰ� <em>say</em> ������Ϊ<em>execute</em>�����ĵ�һ�����������˴��ݡ����ﷵ�صĲ��� <em>say</em> �ķ���ֵ������ <em>say</em> ����
        </p>

        <p>
            ����һ���� <em>say</em> �ͱ����<em>execute</em> �еı��ر��� <em>someFunction</em> ��execute����ͨ������ <em>someFunction()</em> �������ŵ���ʽ����ʹ�� <em>say</em> ������
        </p>

        <p>
            ��Ȼ����Ϊ <em>say</em> ��һ�������� <em>execute</em> �ڵ��� <em>someFunction</em> ʱ���Դ�������һ��������
        </p>

        <p>
            ���ǿ��ԣ�����ղ����������������ְ�һ��������Ϊ�������ݡ��������ǲ�һ��Ҫ��������ȶ��壬�ٴ��ݡ���Ȧ�ӣ����ǿ���ֱ������һ�������������ж���ʹ������������
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> execute</span><span
                class="pun">(</span><span class="pln">someFunction</span><span class="pun">,</span><span class="pln"> value</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; someFunction</span><span
                class="pun">(</span><span class="pln">value</span><span class="pun">);</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>execute</span><span
                class="pun">(</span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">word</span><span class="pun">){</span><span class="pln"> console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span
                class="pln">word</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">},</span><span class="pln"> </span><span class="str">"Hello"</span><span
                class="pun">);</span></pre>

        <p>
            ������ <em>execute</em> ���ܵ�һ�������ĵط�ֱ�Ӷ���������׼�����ݸ� <em>execute</em> �ĺ�����
        </p>

        <p>
            �����ַ�ʽ�������������ø�������������֣���Ҳ��Ϊʲô�������� <em>��������</em> ��
        </p>

        <p>
            �������Ǻ�������Ϊ�ġ����ס�JavaScript�ĵ�һ�����ܽӴ����������ǻ��ǵ�ѭ�򽥽������ڣ������Ƚ�����һ�㣺��JavaScript�У�һ������������Ϊ��һ����������һ�����������ǿ����ȶ���һ��������Ȼ�󴫵ݣ�Ҳ�����ڴ��ݲ����ĵط�ֱ�Ӷ��庯����
        </p>

        <a name="how-function-passing-makes-our-http-server-work"></a>

        <h3>���������������HTTP������������</h3>

        <p>������Щ֪ʶ�����������������Ǽ�Լ�����򵥵�HTTP��������</p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br>http</span><span
                class="pun">.</span><span class="pln">createServer</span><span class="pun">(</span><span class="kwd">function</span><span
                class="pun">(</span><span class="pln">request</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; response</span><span class="pun">.</span><span class="pln">write</span><span
                class="pun">(</span><span class="str">"Hello World"</span><span class="pun">);</span><span
                class="pln"><br>&nbsp; response</span><span class="pun">.</span><span class="pln">end</span><span
                class="pun">();</span><span class="pln"><br></span><span class="pun">}).</span><span
                class="pln">listen</span><span class="pun">(</span><span class="lit">8888</span><span
                class="pun">);</span></pre>

        <p>����������ȥӦ�������˺ࣺܶ������ <em>createServer</em> ����������һ������������  </p>

        <p>�������Ĵ���Ҳ���Դﵽͬ����Ŀ�ģ�  </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; response</span><span class="pun">.</span><span class="pln">write</span><span
                class="pun">(</span><span class="str">"Hello World"</span><span class="pun">);</span><span
                class="pln"><br>&nbsp; response</span><span class="pun">.</span><span class="pln">end</span><span
                class="pun">();</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>http</span><span
                class="pun">.</span><span class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span></pre>

        <p>Ҳ���������Ǹ�����������ˣ�����ΪʲôҪ�����ַ�ʽ�أ�  </p>

        <a name="event-driven-callbacks"></a>

        <h3>�����¼������Ļص�</h3>

        <p>�������ɲ��ûش����ٶ�����˵������������Node.jsԭ���Ĺ�����ʽ�������¼������ģ���Ҳ����Ϊʲô��ô���ԭ��  </p>

        <p>��Ҳ����뻨��ʱ���һ��Felix Geisend?rfer�Ĵ���<a href="http://debuggable.com/posts/understanding-node-js:4bd98440-45e4-4a9a-8ef7-0f7ecbdd56cb">Understanding node.js</a>����������һЩ����֪ʶ��  </p>

        <p>��һ�ж�����ڡ�Node.js���¼������ġ���һ��ʵ���ðɣ���ʵ��Ҳ�����ر�ȷ�е��˽���仰����˼�������һ����Ž��ͣ�Ϊʲô����������Node.jsд����Ӧ�ã�Web based application����������ġ�  </p>

        <p>������ʹ�� <em>http.createServer</em> ������ʱ�����ǵ�Ȼ��ֻ����Ҫһ������ĳ���˿ڵķ����������ǻ���Ҫ���ڷ������յ�һ��HTTP�����ʱ������ʲô��  </p>

        <p>�����ǣ������첽�ģ������κ�ʱ�򶼿��ܵ���������ǵķ�����ȴ����һ���������С�  </p>

        <p>дPHPӦ�õ�ʱ������һ��Ҳ��Ϊ�˵��ģ��κ�ʱ������������ʱ����ҳ��������ͨ����Apache����Ϊ��һ�����½�һ�����̣����ҿ�ʼ��ͷ��βִ����Ӧ��PHP�ű���  </p>

        <p>��ô�����ǵ�Node.js�����У���һ���µ����󵽴�8888�˿ڵ�ʱ��������ô���������أ�  </p>

        <p>�ţ������Node.js/JavaScript���¼���������ܹ���������æ�ĵط��ˡ�����Ȼ���ǻ���ѧһЩ�¸����������������������������Щ��������ôӦ�������ǵķ�����������ġ�  </p>

        <p>���Ǵ����˷������������򴴽����ķ���������һ�����������ۺ�ʱ���ǵķ������յ�һ��������������ͻᱻ���á�  </p>

        <p>���ǲ�֪���������ʲôʱ��ᷢ��������������������һ����������ĵط������������Ǵ��ݹ�ȥ���Ǹ��������������Ǳ�Ԥ�ȶ���ĺ��������������������޹ؽ�Ҫ�ˡ�  </p>

        <p>������Ǵ�˵�е� <em>�ص�</em> �����Ǹ�ĳ������������һ���������������������Ӧ�¼�����ʱ����������������� <em>�ص�</em> ��  </p>

        <p>���ٶ�����˵����ҪһЩ�������Ū��������������ǲ�̫ȷ���Ļ�����ȥ����Felix�Ĳ������¡�  </p>

        <p>������������ĥ��ĥ����¸��������ô֤�����ڴ����������֮�󣬼�ʹû��HTTP������������ǵĻص�����Ҳû�б����õ�����£����ǵĴ��뻹������Ч�أ��������������  </p>

        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request received."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello World"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>http</span><span class="pun">.</span><span class="pln">createServer</span><span
                class="pun">(</span><span class="pln">onRequest</span><span class="pun">).</span><span class="pln">listen</span><span
                class="pun">(</span><span class="lit">8888</span><span class="pun">);</span><span class="pln"><br><br>console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span></pre>

        <p>ע�⣺�� <em>onRequest</em> �����ǵĻص������������ĵط������� <em>console.log</em> �����һ���ı�����HTTP��������ʼ����<em>֮��</em>��Ҳ���һ���ı���  </p>

        <p>
            ������������һ����������<em>node server.js</em>ʱ�������������������������Server has started.������������������������������������<a href="http://localhost:8888/" rel="nofollow">http://localhost:8888/</a> ������Request received.��������Ϣ�ͻ����������г��֡�
        </p>

        <p>������¼��������첽��������JavaScript�����Ļص�����</p>

        <p>����ע�⣬�������ڷ�����������ҳʱ�����ǵķ��������ܻ�������Ρ�Request received.����������Ϊ�󲿷ַ���������������� http://localhost:8888 /ʱ���Զ�ȡ http://localhost:8888/favicon.ico )</p>

        <a name="how-our-server-handles-requests"></a>

        <h3>����������δ��������</h3>

        <p>�õģ����������Ǽ򵥷���һ�����Ƿ�����������ʣ�µĲ��֣�Ҳ�������ǵĻص����� <em>onRequest()</em> �����岿�֡�  </p>

        <p>���ص����������ǵ� <em>onRequest()</em> ������������ʱ�����������������룺 <em>request</em> �� <em>response</em> ��  </p>

        <p>�����Ƕ��������ʹ�����ǵķ���������HTTP�����ϸ�ڣ�������Ӧ���󣨱����򷢳���������������һЩ��������  </p>

        <p>�������ǵĴ�����ǣ����յ�����ʱ��ʹ�� <em>response.writeHead()</em> ��������һ��HTTP״̬200��HTTPͷ���������ͣ�content-type����ʹ�� <em>response.write()</em> ������HTTP��Ӧ�����з����ı���Hello World"��  </p>

        <p>������ǵ��� <em>response.end()</em> �����Ӧ��  </p>

        <p>Ŀǰ��˵�����Ƕ������ϸ�ڲ������⣬��������û��ʹ�� <em>request</em> ����  </p>

        <a name="finding-a-place-for-our-server-module"></a>

        <h3>����˵�ģ���������</h3>

        <p>OK�������ұ�֤�����������������ڿ��Իص����������֯Ӧ������������ˡ����������� <em>server.js</em> �ļ�����һ���ǳ�������HTTP���������룬�������ᵽͨ�����ǻ���һ���� <em>index.js</em> ���ļ�ȥ����Ӧ�õ�����ģ�飨���� <em>server.js</em> �е�HTTP������ģ�飩������������Ӧ�á�  </p>

        <p>�������ھ���̸̸��ô��server.js���һ��������Node.jsģ�飬ʹ�����Ա����ǣ���û�������� <em>index.js</em> ���ļ�ʹ�á�</p>

        <p>Ҳ�����Ѿ�ע�⵽�������Ѿ��ڴ�����ʹ����ģ���ˡ���������  </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br></span><span class="pun">...</span><span
                class="pln"><br><br>http</span><span class="pun">.</span><span class="pln">createServer</span><span
                class="pun">(...);</span></pre>

        <p>Node.js���Դ���һ��������http����ģ�飬���������ǵĴ��������������ѷ���ֵ����һ�����ر�����  </p>

        <p>������ǵı��ر��������һ��ӵ������ <em>http</em> ģ�����ṩ�Ĺ��������Ķ���</p>

        <p>�����ֱ��ر�����һ����ģ������һ����������һ�ֹ�����������Ҳ���԰����Լ���ϲ������  </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> foo </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br></span><span class="pun">...</span><span
                class="pln"><br><br>foo</span><span class="pun">.</span><span class="pln">createServer</span><span
                class="pun">(...);</span></pre>

        <p>�ܺã���ôʹ��Node.js�ڲ�ģ���Ѿ�������ˡ�������ô�����Լ���ģ�飬����ôʹ�����أ�  </p>

        <p>�����ǰ� <em>server.js</em> ���һ��������ģ�飬����ܸ������ˡ�  </p>

        <p>��ʵ�ϣ����ǲ�����̫����޸ġ���ĳ�δ�����ģ����ζ��������Ҫ������ϣ���ṩ�书�ܵĲ��� <em>����</em> ���������ģ��Ľű���  </p>

        <p>Ŀǰ�����ǵ�HTTP��������Ҫ�����Ĺ��ܷǳ��򵥣���Ϊ���������ģ��Ľű���������Ҫ�������������ѡ�  </p>

        <p>���ǰ����ǵķ������ű��ŵ�һ������ <em>start</em> �ĺ����Ȼ�����ǻᵼ�����������  </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; </span><span class="kwd">function</span><span class="pln"> onRequest</span><span
                class="pun">(</span><span class="pln">request</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request received."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello World"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>�������������ھͿ��Դ������ǵ����ļ� <em>index.js</em> ���������������ǵ�HTTP�ˣ���Ȼ�������Ĵ��뻹�� <em>server.js</em> �С�  </p>

        <p>���� <em>index.js</em> �ļ���д���������ݣ�  </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> server </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"./server"</span><span
                class="pun">);</span><span class="pln"><br><br>server</span><span class="pun">.</span><span class="pln">start</span><span
                class="pun">();</span></pre>

        <p>�������������ģ����ǿ�����ʹ���κ�����������ģ��һ��ʹ��serverģ�飺��������ļ�������ָ��һ�������������ѵ����ĺ����Ϳ��Ա�����ʹ���ˡ�</p>

        <p>���ˡ��������ھͿ��Դ����ǵ���Ҫ�ű��������ǵĵ�Ӧ���ˣ��������������ӣ�</p>
        <pre>node index.js</pre>

        <p>�ǳ��ã��������ڿ��԰����ǵ�Ӧ�õĲ�ͬ���ַ��벻ͬ���ļ������ͨ������ģ��ķ�ʽ���������ӵ�һ���ˡ�  </p>

        <p>������Ȼֻӵ������Ӧ�õ�������֣����ǿ��Խ���HTTP���󡣵������ǵ�����ʲô�������ڲ�ͬ��URL���󣬷�����Ӧ���в�ͬ�ķ�Ӧ��  </p>

        <p>����һ���ǳ��򵥵�Ӧ����˵�������ֱ���ڻص����� <em>onRequest()</em> ����������顣����������˵���ģ�����Ӧ�ü���һЩ�����Ԫ�أ������ǵ����ӱ�ø���Ȥһ�����  </p>

        <p>����ͬ��HTTP���������ǵĴ�������һ����ͬ�Ĳ��֣�������·��ѡ�񡱡�����ô�����ǽ������ʹ���һ������ <em>·��</em> ��ģ��ɡ�  </p>

        <a name="whats-needed-to-route-requests"></a>

        <h3>�������������ġ�·�ɡ�</h3> 

         <p>����ҪΪ·���ṩ�����URL��������Ҫ��GET��POST���������·����Ҫ������Щ������ִ����Ӧ�Ĵ��루������롱��Ӧ����Ӧ�õĵ������֣�һϵ���ڽ��յ�����ʱ���������Ĵ�����򣩡�</p>

        <p>��ˣ�������Ҫ�鿴HTTP���󣬴�����ȡ�������URL�Լ�GET/POST��������һ����Ӧ������·�ɻ��Ƿ�������������Ϊһ��ģ������Ĺ��ܣ�ȷʵֵ��̽�֣��������ݶ���Ϊ���ǵ�HTTP�������Ĺ��ܡ�</p>

        <p>������Ҫ���������ݶ��������request�����У��ö�����Ϊ<em>onRequest()</em>�ص������ĵ�һ���������ݡ�����Ϊ�˽�����Щ���ݣ�������Ҫ�����Node.JSģ�飬���Ƿֱ���<em>url</em>��<em>querystring</em>ģ�顣</p>
<pre>                               url.parse(string).query
                                           |
           url.parse(string).pathname      |
                       |                   |
                       |                   |
                     ------ -------------------
http://localhost:8888/start?foo=bar&amp;hello=world
                                ---       -----
                                 |          |
                                 |          |
              querystring(string)["foo"]    |
                                            |
                         querystring(string)["hello"]
</pre>

        <p>��Ȼ����Ҳ������<em>querystring</em>ģ��������POST�������еĲ������Ժ������ʾ��</p>

        <p>������������<em>onRequest()</em>��������һЩ�߼��������ҳ�����������URL·����</p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; </span><span class="kwd">function</span><span class="pln"> onRequest</span><span
                class="pun">(</span><span class="pln">request</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello World"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>���ˣ����ǵ�Ӧ�����ڿ���ͨ�������URL·��������ͬ������--��ʹ���ǵ���ʹ��·�ɣ���δ��ɣ�����������URL·��Ϊ��׼ӳ�䵽��������ϡ�</p>

        <p>��������Ҫ������Ӧ���У�����ζ������<em>/start</em>��<em>/upload</em>���������ʹ�ò�ͬ�Ĵ����������Ժ����ǽ�������Щ������������ϵ�һ��ġ�</p>

        <p>�������ǿ�������д·���ˣ�����һ����Ϊ<em>router.js</em>���ļ�������������ݣ�</p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> route</span><span
                class="pun">(</span><span class="pln">pathname</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"About to route a request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">route </span><span class="pun">=</span><span
                class="pln"> route</span><span class="pun">;</span></pre>

        <p>������������δ���ʲôҲû�ɣ���������������˵����Ӧ�õġ�����Ӹ�����߼���ǰ����������������ΰ�·�ɺͷ���������������</p>

        <p>���ǵķ�����Ӧ��֪��·�ɵĴ��ڲ�������Ч���á����ǵ�Ȼ����ͨ��Ӳ����ķ�ʽ����һ������󶨵��������ϣ������������Եı�̾���������������һ���ǳ�ʹ����£�������ǽ�ʹ������ע��ķ�ʽ����ɢ�����·��ģ�飨����Զ���<a href="http://martinfowler.com/articles/injection.html">Martin Fowlers��������ע��Ĵ���</a>����Ϊ����֪ʶ����</p>

        <p>���ȣ���������չһ�·�������<em>start()</em>�������Ա㽫·�ɺ�����Ϊ�������ݹ�ȥ��</p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">route</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; </span><span class="kwd">function</span><span class="pln"> onRequest</span><span
                class="pun">(</span><span class="pln">request</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; &nbsp; route</span><span class="pun">(</span><span
                class="pln">pathname</span><span class="pun">);</span><span
                class="pln"><br><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello World"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>ͬʱ�����ǻ���Ӧ��չ<em>index.js</em>��ʹ��·�ɺ������Ա�ע�뵽�������У�</p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> server </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"./server"</span><span
                class="pun">);</span><span class="pln"><br></span><span class="kwd">var</span><span
                class="pln"> router </span><span class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"./router"</span><span class="pun">);</span><span class="pln"><br><br>server</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">(</span><span
                class="pln">router</span><span class="pun">.</span><span class="pln">route</span><span
                class="pun">);</span><span class="pln"><br></span></pre>

        <p>��������Ǵ��ݵĺ�������ʲôҲû����</p>

        <p>�����������Ӧ�ã�<em>node index.js��ʼ�ռǵ����������</em>�����������һ��URL���㽫�ῴ��Ӧ�������Ӧ����Ϣ����������ǵ�HTTP�������Ѿ���ʹ��·��ģ���ˣ����Ὣ�����·�����ݸ�·�ɣ�</p>

        <pre>bash$ node index.js
Request for /foo received.
About to route a request for /foo</pre>

        <p>����������Ѿ�ȥ���˱ȽϷ��˵�/favicon.ico������صĲ��֣���</p>
 
        <a name="execution-in-the-kongdom-of-verbs"></a> 
 
        <h3>��Ϊ����ִ��</h3> 

        <p>���������ٴ��������⣬������̸һ̸����ʽ��̡�</p>

        <p>��������Ϊ�������ݲ����������ڼ����ϵĿ���������������˵������ʵ�Ǹ���ѧ���⡣���������ĳ�������index�ļ��У����ǿ��Խ�<em>router</em>���󴫵ݽ�ȥ�������������Ե�����������<em>route</em>������</p>

        <p>�������������Ǵ���һ��������Ȼ�����������������������һЩ�¡����Ǹ���·�ɵĶ������ܰ��Ұ����·��һ����</p>

        <p>���Ƿ�������ʵ����Ҫ�����Ķ�������ֻ��Ҫ������������У���ʵΪ�˰��������꣬���������Ҫ����������Ҫ���Ƕ�����Ҳ����˵���㲻��Ҫ<em>����</em>������Ҫ<em>����</em>��</p>

        <p>������������������ġ��������˼��ת��������Ȼ��Ȼ������˺�����̡�</p>

        <p>�����ڶ���Steve Yegge�Ĵ���<a href="http://steve-yegge.blogspot.com/2006/03/execution-in-kingdom-of-nouns.html">���������е�����</a>֮����⺯����̡���Ҳȥ��һ���Ȿ��ɣ���ġ��������������Ķ��Ŀ��ֵĹ���������鼮֮һ��</p>

        <a name="routing-to-real-request-handlers"></a> 
 
        <h3>·�ɸ����������������</h3> 

         <p>�ص����⣬�������ǵ�HTTP������������·��ģ���Ѿ������ǵ������������໥�����ˣ�����һ�������޼���ֵܡ�</p>

        <p>��Ȼ�⻹ԶԶ������·�ɣ�����˼�壬��ָ����Ҫ��Բ�ͬ��URL�в�ͬ�Ĵ���ʽ�����紦��<em>/start</em>�ġ�ҵ���߼�����Ӧ�úʹ���<em>/upload</em>�Ĳ�ͬ��</p>

        <p>�����ڵ�ʵ���£�·�ɹ��̻���·��ģ���С�������������·��ģ�鲢��������������󡰲�ȡ�ж�����ģ�飬�������ǵ�Ӧ�ó����ø�Ϊ����ʱ�����޷��ܺõ���չ��</p>

        <p>������ʱ����Ϊ·��Ŀ��ĺ�����Ϊ����������������ǲ�Ҫ����������·��ģ�飬��Ϊ������������û�о����Ļ�������ô����·��ģ��Ҳû�ж�����塣</p>

        <p>Ӧ�ó�����Ҫ�µĲ�������˼����µ�ģ�� -- �Ѿ�����Ϊ�˸е������ˡ�����������һ������requestHandlers��ģ�飬������ÿһ��������������һ��ռλ�ú����������Щ������Ϊģ��ķ���������</p>

        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span
                class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>�������ǾͿ��԰�����������·��ģ��������������·�ɡ���·��Ѱ����</p>

        <p>���������ǵ������������ǽ�requestHandlersģ��Ӳ���뵽·������ʹ�ã����������һ������ע�룿��Ȼ������ģʽһ��������ע�벻Ӧ�ý���Ϊʹ�ö�ʹ�ã����������������£�ʹ������ע�������·�ɺ����������֮�����ϸ�����ɢ��Ҳ�������·�ɵ������Ը��ߡ�</p>

        <p>����ζ�����ǵý����������ӷ��������ݵ�·���У����о�����ô���������ˣ����ǵ�һ·������������������ǵ����ļ����ݵ��������У��ٽ�֮�ӷ��������ݵ�·�ɡ�</p>

        <p>��ô����Ҫ��ô������Щ����������أ�����������ֻ��2�����������һ����ʵ��Ӧ���У����������������᲻�����ӣ����ǵ�Ȼ����ÿ����һ���µ�URL�����������ʱ����ҪΪ����·����������󵽴�������ӳ����������ڡ�����֮�⣬��·������һ���<em>if request == x then call handler y</em>Ҳʹ��ϵͳ��ª������</p>

        <p>��ϸ���룬��һ��Ѷ�����ÿ����Ҫӳ�䵽һ���ַ��������������URL���ϣ��ƺ��������飨associative array��������ʤ�Ρ�</p>

        <p>��������е�����ʧ����JavaScriptû�ṩ�������� -- Ҳ����˵���ṩ�ˣ���ʵ�ϣ���JavaScript�У��������ṩ���๦�ܵ������Ķ���</p>

        <p>���ⷽ�棬<a href="http://msdn.microsoft.com/en-us/magazine/cc163419.aspx">http://msdn.microsoft.com/en-us/magazine/cc163419.aspx</a>��һ������Ľ��ܣ����ڴ�ժ¼һ�Σ�</p>

         <blockquote>
            <p>��C++��C#�У�������̸������ָ��������߽ṹ���ʵ���������������ʵ������ģ�壨������ν���ࣩ����ӵ�в�ͬ�����Ժͷ���������JavaScript���������������JavaScript�У��������һ����/ֵ�Եļ��� -- ����԰�JavaScript�Ķ��������һ����Ϊ�ַ������͵��ֵ䡣</p>
        </blockquote>

        <p>�����JavaScript�Ķ�������Ǽ�/ֵ�Եļ��ϣ�������ô��ӵ�з����أ��ðɣ������ֵ�������ַ��������ֻ��ߡ���������</p>

        <p>���ˣ�����ٻص��������������������Ѿ�ȷ����һϵ�����������ͨ��һ�����������ݣ�������Ҫʹ������ϵķ�ʽ���������ע�뵽<em>route()</em>�����С�</p>

        <p>�����Ƚ�����������뵽���ļ�<em>index.js</em>�У�</p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> server </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"./server"</span><span
                class="pun">);</span><span class="pln"><br></span><span class="kwd">var</span><span
                class="pln"> router </span><span class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"./router"</span><span class="pun">);</span><span class="pln"><br></span><span class="kwd">var</span><span
                class="pln"> requestHandlers </span><span class="pun">=</span><span class="pln"> require</span><span
                class="pun">(</span><span class="str">"./requestHandlers"</span><span class="pun">);</span><span
                class="pln"><br><br></span><span class="kwd">var</span><span class="pln"> handle </span><span
                class="pun">=</span><span class="pln"> </span><span class="pun">{}</span><span
                class="pln"><br>handle</span><span class="pun">[</span><span class="str">"/"</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">=</span><span class="pln"> requestHandlers</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">;</span><span class="pln"><br>handle</span><span
                class="pun">[</span><span class="str">"/start"</span><span class="pun">]</span><span
                class="pln"> </span><span class="pun">=</span><span class="pln"> requestHandlers</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">;</span><span class="pln"><br>handle</span><span
                class="pun">[</span><span class="str">"/upload"</span><span class="pun">]</span><span
                class="pln"> </span><span class="pun">=</span><span class="pln"> requestHandlers</span><span
                class="pun">.</span><span class="pln">upload</span><span class="pun">;</span><span class="pln"><br><br>server</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">(</span><span
                class="pln">router</span><span class="pun">.</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">);</span></pre>

        <p>��Ȼ<em>handle</em>����������һ������������һЩ���������ļ��ϣ����һ��ǽ�����һ��������Ϊ��������������������������·����ʹ�ø������ı��ʽ���Ժ����˵����</p>

        <p>��������������ͬ��URLӳ�䵽��ͬ��������������Ǻ����׵ģ�ֻҪ�ڶ��������һ����Ϊ<em>"/"</em>�����ԣ���Ӧ<em>requestHandlers.start</em>���ɣ��������ǾͿ��Ըɾ���������<em>/start</em>��<em>/</em>�����󶼽���<em>start</em>��һ���������</p>

        <p>������˶���Ķ�������ǰ�����Ϊ����Ĳ������ݸ���������Ϊ�˽�<em>server.js</em>�޸����£�</p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; </span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; &nbsp; route</span><span class="pun">(</span><span
                class="pln">handle</span><span class="pun">,</span><span class="pln"> pathname</span><span class="pun">);</span><span
                class="pln"><br><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello World"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>�������Ǿ���<em>start()</em>�����������<em>handle</em>���������Ұ�handle������Ϊ��һ���������ݸ���<em>route()</em>�ص�������</p>

        <p>Ȼ��������Ӧ����<em>route.js</em>�ļ����޸�<em>route()</em>������</p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> route</span><span
                class="pun">(</span><span class="pln">handle</span><span class="pun">,</span><span
                class="pln"> pathname</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span class="str">"About to route a request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">if</span><span
                class="pln"> </span><span class="pun">(</span><span class="kwd">typeof</span><span
                class="pln"> handle</span><span class="pun">[</span><span class="pln">pathname</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">===</span><span
                class="pln"> </span><span class="str">'function'</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; handle</span><span
                class="pun">[</span><span class="pln">pathname</span><span class="pun">]();</span><span class="pln"><br>&nbsp; </span><span
                class="pun">}</span><span class="pln"> </span><span class="kwd">else</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"No request handler found for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">route </span><span class="pun">=</span><span
                class="pln"> route</span><span class="pun">;</span></pre>

       <p>ͨ�����ϴ��룬�������ȼ�������·����Ӧ������������Ƿ���ڣ�������ڵĻ�ֱ�ӵ�����Ӧ�ĺ��������ǿ����ôӹ��������л�ȡԪ��һ���ķ�ʽ�Ӵ��ݵĶ����л�ȡ������������˾����˼������������<em>handle&#91;pathname&#93;();</em>�ı��ʽ������о�������ǰ�����ᵽ�����������ˣ�����Ҵ��������·������</p>

        <p>������Щ�����ǾͰѷ�������·�ɺ������������һ���ˡ�������������Ӧ�ó�����������з���<em>http://localhost:8888/start</em>��������־����˵��ϵͳ��������ȷ�����������</p>

        <pre>Server has started.
Request for /start received.
About to route a request for /start
Request handler 'start' was called.</pre>

         <p>������������д�<em>http://localhost:8888/</em>���Կ����������ͬ����<em>start</em>������������ˣ�</p>
        <pre>Request for / received.
About to route a request for /
Request handler 'start' was called.</pre>

        <a name="making-the-request-handlers-respond"></a>

        <h3>�����������������Ӧ</h3>

        <p>
            �ܺá���������Ҫ������������ܹ������������һЩ���������Ϣ������ȫ�ǡ�Hello World�����Ǿ͸����ˡ�
        </p>

        <p>
            ����Ҫ��ס���ǣ����������������ò���ʾ�ġ�Hello World����Ϣ��������������<em>server.js</em>�ļ��е�<em>onRequest</em>������
        </p>

        <p>
            ��ʵ����������˵���˾��ǡ�������������Ӧ������ˣ�������Ҫ������������ܹ���<em>onRequest</em>�����������Ժ���������С��Ի�����
        </p>

        <a name="how-to-not-do-it"></a>

        <h4>���õ�ʵ�ַ�ʽ</h4>

        <p>
            ������������ӵ��PHP����Ruby���������Ŀ�������˵����ֱ���˵���ʵ�ַ�ʽ��ʵ�ϲ����Ƿǳ����ף� ������Ч��ʵ��δ����ˡ�
        </p>

        <p>
            ������ָ�ġ�ֱ���˵���ʵ�ַ�ʽ����˼�ǣ������������ͨ��<em>onRequest</em>����ֱ�ӷ��أ�<em>return()</em>������Ҫչʾ���û�����Ϣ��
        </p>

        <p>
            �����Ⱦ�����ȥʵ�֣�Ȼ��������Ϊʲô�ⲻ��һ�ֺܺõ�ʵ�ַ�ʽ��
        </p>

        <p>
            �����Ǵ�����������򷵻���Ҫ�����������ʾ����Ϣ��ʼ��������Ҫ��<em>requestHandler.js</em>�޸�Ϊ������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">return</span><span
                class="pln"> </span><span class="str">"Hello Start"</span><span class="pun">;</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> upload</span><span class="pun">()</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span
                class="str">"Request handler 'upload' was called."</span><span class="pun">);</span><span
                class="pln"><br>&nbsp; </span><span class="kwd">return</span><span class="pln"> </span><span
                class="str">"Hello Upload"</span><span class="pun">;</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>exports</span><span class="pun">.</span><span class="pln">start </span><span
                class="pun">=</span><span class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            �õġ�ͬ���ģ�����·����Ҫ����������򷵻ظ�������Ϣ���ظ�����������ˣ�������Ҫ��<em>router.js</em>�޸�Ϊ������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> route</span><span
                class="pun">(</span><span class="pln">handle</span><span class="pun">,</span><span
                class="pln"> pathname</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span class="str">"About to route a request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">if</span><span
                class="pln"> </span><span class="pun">(</span><span class="kwd">typeof</span><span
                class="pln"> handle</span><span class="pun">[</span><span class="pln">pathname</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">===</span><span
                class="pln"> </span><span class="str">'function'</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">return</span><span class="pln"> handle</span><span class="pun">[</span><span class="pln">pathname</span><span
                class="pun">]();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"> </span><span class="kwd">else</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span class="str">"No request handler found for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="kwd">return</span><span
                class="pln"> </span><span class="str">"404 Not found"</span><span class="pun">;</span><span class="pln"><br>&nbsp; </span><span
                class="pun">}</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">route </span><span class="pun">=</span><span
                class="pln"> route</span><span class="pun">;</span></pre>
        <p>
            ��������������ʾ���������޷�·�ɵ�ʱ������Ҳ������һЩ��صĴ�����Ϣ��
        </p>

        <p>
            ���������Ҫ�����ǵ�<em>server.js</em>�����ع���ʹ�����ܹ������������ͨ������·�ɷ��ص�������Ӧ���������������ʾ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; </span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="kwd">var</span><span class="pln"> content </span><span
                class="pun">=</span><span class="pln"> route</span><span class="pun">(</span><span
                class="pln">handle</span><span class="pun">,</span><span class="pln"> pathname</span><span
                class="pun">)</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">content</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>
        <p>
            ������������ع����Ӧ�ã�һ�ж��Ṥ���ĺܺã�����<a href="http://localhost:8888/start" rel="nofollow">http://localhost:8888/start</a>,������������Hello Start��������<a href="http://localhost:8888/upload" rel="nofollow">http://localhost:8888/upload</a>�������Hello Upload��,������<a href="http://localhost:8888/foo" rel="nofollow">http://localhost:8888/foo</a> �������404 Not found����
        </p>

        <p>
            �ã���ô�����������أ��򵥵�˵���ǣ� ��δ���������������Ҫ���з������Ĳ�����ʱ�����ǵ�Ӧ�þ͡��ҡ��ˡ�
        </p>

        <p>
            û��⣿û��ϵ�����������ϸ�����¡�
        </p>

        <a name="blocking-and-non-blocking"></a>

        <h4>�����������</h4>

        <p>
            �����ǰ���ᵽ�ģ���������������а�������������ʱ�ͻ�����⡣���ǣ���˵��֮ǰ��������������ʲô������������
        </p>

        <p>
            �Ҳ���ȥ���͡��������͡����������ľ��庬�壬����ֱ����������������������м�����������ʱ�ᷢ��ʲô��
        </p>

        <p>
            ����������޸���<em>start</em>������������������ȴ�10���Ժ��ٷ��ء�Hello Start������Ϊ��JavaScript��û������<em>sleep()</em>�����Ĳ�������������ֻ�ܹ�����СHack��ģ��ʵ�֡�
        </p>

        <p>
            �����ǽ�<em>requestHandlers.js</em>�޸ĳ�������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">function</span><span
                class="pln"> sleep</span><span class="pun">(</span><span class="pln">milliSeconds</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> startTime </span><span class="pun">=</span><span
                class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span
                class="typ">Date</span><span class="pun">().</span><span class="pln">getTime</span><span
                class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="kwd">while</span><span
                class="pln"> </span><span class="pun">(</span><span class="kwd">new</span><span
                class="pln"> </span><span class="typ">Date</span><span class="pun">().</span><span
                class="pln">getTime</span><span class="pun">()</span><span class="pln"> </span><span
                class="pun">&lt;</span><span class="pln"> startTime </span><span class="pun">+</span><span class="pln"> milliSeconds</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; sleep</span><span class="pun">(</span><span class="lit">10000</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">return</span><span
                class="pln"> </span><span class="str">"Hello Start"</span><span class="pun">;</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> upload</span><span class="pun">()</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span
                class="str">"Request handler 'upload' was called."</span><span class="pun">);</span><span
                class="pln"><br>&nbsp; </span><span class="kwd">return</span><span class="pln"> </span><span
                class="str">"Hello Upload"</span><span class="pun">;</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>exports</span><span class="pun">.</span><span class="pln">start </span><span
                class="pun">=</span><span class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ���������У�������<em>start()</em>�����õ�ʱ��Node.js���ȵȴ�10�룬֮��Ż᷵�ء�Hello Start����������<em>upload()</em>��ʱ�򣬻�ʹ�ǰһ���������ء�
        </p>

        <p>
            ����Ȼ�ˣ�����ֻ��ģ������10�룬ʵ�ʳ����У����������������кܶ࣬�ȷ�˵һЩ��ʱ��ļ�������ȡ���
        </p>

        <p>
            �������������������������ǵĸĶ���������Щ�仯��
        </p>

        <p>
            ������һ����������Ҫ�����·�������Ϊ�˿���Ч��������Ҫ����һЩ��Ը��ӵĲ�����������һ�������� ���ȣ���������������ڻ��߱�ǩҳ���ڵ�һ����������ڵĵ�ַ��������<a href="http://localhost:8888/start" rel="nofollow">http://localhost:8888/start</a>�� �����Ȳ�Ҫ������
        </p>

        <p>
            �ڵڶ�����������ڵĵ�ַ��������<a href="http://localhost:8888/upload" rel="nofollow">http://localhost:8888/upload</a>�� ͬ���ģ��Ȳ�Ҫ������
        </p>

        <p>
           �������������²������ڵ�һ�������У���/start�������»س���Ȼ������л����ڶ��������У���/upload�������»س���
        </p>

        <p>
            ע�⣬������ʲô�� /start URL���ػ���10�룬�������Ԥ�ڵ�һ�������ǣ�/upload URL��Ȼ<em>Ҳ</em>����10�룬�����ڶ�Ӧ������������в�û��������<em>sleep()</em>�����Ĳ�����
        </p>

        <p>
            �⵽����Ϊʲô�أ�ԭ�����<em>start()</em>���������������������˵���ǡ������������������Ĵ���������
        </p>

        <p>
            ����Ȼ�Ǹ����⣬��ΪNodeһ��������������Լ��ģ�<em>����node�г��˴��룬����һ�ж��ǲ���ִ�еġ�</em>��
        </p>

        <p>
            ��仰����˼��˵��Node.js�����ڲ����������̵߳�����£���Ȼ���Զ�������в��д��� ���� Node.js�ǵ��̵߳ġ���ͨ���¼���ѯ��event loop����ʵ�ֲ��в������Դˣ�����Ӧ��Ҫ���������һ�� ���� �����ܵı�������������ȡ����֮����ʹ�÷�����������
        </p>

        <p>
            Ȼ����Ҫ�÷�����������������Ҫʹ�ûص���ͨ����������Ϊ�������ݸ�������Ҫ��ʱ��������ĺ������ȷ�˵������10�룬���߲�ѯ���ݿ⣬�ֻ����ǽ��д����ļ��㣩��
        </p>

        <p>
            ����Node.js��˵��������������ģ�<em>���٣�probablyExpensiveFunction()������ע������ָ�ľ�����Ҫ��ʱ�䴦��ĺ����������������������飬�ң�Node.js�̣߳��Ȳ������ˣ��Ҽ���ȥ���������Ĵ��룬�����ṩһ��callbackFunction()�����㴦����֮���һ�ȥ���øûص������ģ�лл����</em>
        </p>

        <p>
            �������Ҫ�˽��������¼���ѯϸ�ڣ������Ķ�Mixu�Ĳ��ġ���<a href="http://blog.mixu.net/2011/02/01/understanding-the-node-js-event-loop/">���node.js���¼���ѯ</a>����
        </p>

        <p>
            �����������ǻ����һ�ִ����ʹ�÷����������ķ�ʽ��
        </p>

        <p>
            ���ϴ�һ��������ͨ���޸����ǵ�Ӧ������¶���⡣
        </p>

        <p>
            ������ǻ�����<em>start</em>��������������������������޸ĳ�������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> exec </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"child_process"</span><span
                class="pun">).</span><span class="pln">exec</span><span class="pun">;</span><span
                class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">var</span><span class="pln"> content </span><span
                class="pun">=</span><span class="pln"> </span><span class="str">"empty"</span><span class="pun">;</span><span
                class="pln"><br><br>&nbsp; exec</span><span class="pun">(</span><span class="str">"ls -lah"</span><span
                class="pun">,</span><span class="pln"> </span><span class="kwd">function</span><span
                class="pln"> </span><span class="pun">(</span><span class="pln">error</span><span
                class="pun">,</span><span class="pln"> stdout</span><span class="pun">,</span><span
                class="pln"> stderr</span><span class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; &nbsp; content </span><span class="pun">=</span><span
                class="pln"> stdout</span><span class="pun">;</span><span class="pln"><br>&nbsp; </span><span
                class="pun">});</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">return</span><span
                class="pln"> content</span><span class="pun">;</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">return</span><span
                class="pln"> </span><span class="str">"Hello Upload"</span><span class="pun">;</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ���������У�����������һ���µ�Node.jsģ�飬<em>child_process</em>��֮������������Ϊ��ʵ��һ���ȼ���ʵ�õķ�����������<em>exec()</em>��
        </p>

        <p>
            <em>exec()</em>����ʲô�أ�����Node.js��ִ��һ��shell��������������У�������������ȡ��ǰĿ¼�����е��ļ�����ls -lah����,Ȼ�󣬵�<em>/start</em>URL�����ʱ���ļ���Ϣ�����������С�
        </p>

        <p>
            ���������Ƿǳ�ֱ�۵ģ� ������һ���µı���<em>content</em>����ʼֵΪ��empty������ִ�С�ls -lah������������ֵ��content�����content���ء�
        </p>

        <p>
            ������һ��������������������Ȼ����ʡ�<a href="http://localhost:8888/start" rel="nofollow">http://localhost:8888/start</a>�� ��
        </p>

        <p>
            ֮�������һ��Ư����webҳ�棬������Ϊ��empty������ô���£�
        </p>

        <p>
            ���ʱ������ܴ����Ѿ��µ��ˣ�<em>exec()</em>�ڷ�������鷢��������Ĺ�Ч������ʵ�Ǹ��ܺõĶ����������������ǿ���ִ�зǳ���ʱ��shell������������ʹ���ǵ�Ӧ��ͣ�����ȴ��ò�����
        </p>

        <p>
            �������Ҫ֤����һ�㣬���Խ���ls -lah�����ɱ��硰find /����������ʱ�Ĳ�����Ч������
        </p>

        <p>
            Ȼ��������������ʾ�Ľ�����������ǲ����������ǵķ������������԰ɣ�
        </p>

        <p>
            �ã�������������������������⡣��������У���������������Ϊʲô��ǰ�����ַ�ʽ�������á�
        </p>

        <p>
            ��������ڣ�Ϊ�˽��з�����������<em>exec()</em>ʹ���˻ص�������
        </p>

        <p>
            �����ǵ������У��ûص�����������Ϊ�ڶ����������ݸ�<em>exec()</em>������������
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> </span><span
                class="pun">(</span><span class="pln">error</span><span class="pun">,</span><span
                class="pln"> stdout</span><span class="pun">,</span><span class="pln"> stderr</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; content </span><span
                class="pun">=</span><span class="pln"> stdout</span><span class="pun">;</span><span
                class="pln"><br></span><span class="pun">}</span></pre>

        <p>
            ���ھ͵��������Դ�����ˣ����ǵĴ�����ͬ��ִ�еģ������ζ���ڵ���<em>exec()</em>֮��Node.js������ִ�� <em>return content</em> �������ʱ��<em>content</em>��Ȼ�ǡ�empty������Ϊ���ݸ�<em>exec()</em>�Ļص�������δִ�е�������Ϊ<em>exec()</em>�Ĳ������첽�ġ�
        </p>

        <p>
            �������ls -lah���Ĳ�����ʵ�Ƿǳ���ģ����ǵ�ǰĿ¼�����ϰ�����ļ�������Ҳ��Ϊʲô�ص�����Ҳ��ܿ��ִ�е� ���� ������������ô˵�������첽�ġ�
        </p>

        <p>
            Ϊ����Ч���������ԣ���������һ������ʱ����� ��find /���������һ�������Ҫִ��1�������ҵ�ʱ�䣬Ȼ��������������������У��Ұѡ�ls -lah�����ɡ�find /��������/start URL��ʱ����Ȼ�ܹ��������HTTP��Ӧ ���� �����ԣ���<em>exec()</em>�ں�ִ̨�е�ʱ��Node.js��������ִ�к���Ĵ��롣��������������贫�ݸ�<em>exec()</em>�Ļص�������ֻ���ڡ�find /������ִ�����֮��Żᱻ���á�
        </p>

        <p>
            �Ǿ�������Ҫ��β���ʵ�ֽ���ǰĿ¼�µ��ļ��б���ʾ���û��أ�
        </p>

        <p>
            �ã��˽������ֲ��õ�ʵ�ַ�ʽ֮�����ǽ������������������ȷ�ķ�ʽ���������������������������Ӧ��
        </p>

        <a name="responding-request-handlers-with-non-blocking-operations"></a>

        <h4>�Է�������������������Ӧ</h4>

        <p>
            �Ҹո��ᵽ������һ������ ���� ����ȷ�ķ�ʽ��������ʵ��ͨ������ȷ�ķ�ʽ��һ�㶼���򵥡�
        </p>

        <p>
            ��������Node.js��������һ��ʵ�ַ����� �������ݡ�����������������忴�����ʵ�֡�
        </p>

        <p>
            ��ĿǰΪֹ�����ǵ�Ӧ���Ѿ�����ͨ��Ӧ�ø���֮�䴫��ֵ�ķ�ʽ����������� -&gt ����·�� -&gt ������������������򷵻ص����ݣ��������������Ҫ��ʾ���û������ݣ����ݸ�HTTP��������
        </p>

        <p>
            �������ǲ������������µ�ʵ�ַ�ʽ����Բ��ý����ݴ��ݸ��������ķ�ʽ��������β��ý������������ݡ������ݵķ�ʽ�� ��ʵ���Ƕ���˵�����ǽ�<em>response</em>���󣨴ӷ������Ļص�����<em>onRequest()</em>��ȡ��ͨ������·�ɴ��ݸ���������� ��󣬴������Ϳ��Բ��øö����ϵĺ�����������������Ӧ��
        </p>

        <p>
            ԭ�������ˣ���������������һ����ʵ�����ַ�����
        </p>

        <p>
            �ȴ�<em>server.js</em>��ʼ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; </span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; &nbsp; route</span><span class="pun">(</span><span
                class="pln">handle</span><span class="pun">,</span><span class="pln"> pathname</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">);</span><span class="pln"><br>&nbsp; </span><span
                class="pun">}</span><span class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>
            ��Դ�ǰ��<em>route()</em>������ȡ����ֵ��������������ǽ�response������Ϊ�������������ݸ�<em>route()</em>���������ң����ǽ�<em>onRequest()</em>��������������й�<em>response</em>�ĺ��������Ƴ�����Ϊ����ϣ���ⲿ�ֹ�����<em>route()</em>��������ɡ�
        </p>

        <p>
            ��������������ǵ�<em>router.js</em>:
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> route</span><span
                class="pun">(</span><span class="pln">handle</span><span class="pun">,</span><span
                class="pln"> pathname</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"About to route a request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">if</span><span
                class="pln"> </span><span class="pun">(</span><span class="kwd">typeof</span><span
                class="pln"> handle</span><span class="pun">[</span><span class="pln">pathname</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">===</span><span
                class="pln"> </span><span class="str">'function'</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; handle</span><span
                class="pun">[</span><span class="pln">pathname</span><span class="pun">](</span><span class="pln">response</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"> </span><span class="kwd">else</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span class="str">"No request handler found for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">404</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"404 Not found"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">route </span><span class="pun">=</span><span
                class="pln"> route</span><span class="pun">;</span></pre>

        <p>
            ͬ����ģʽ����Դ�ǰ������������л�ȡ����ֵ�����ȡ����֮����ֱ�Ӵ���<em>response</em>����
        </p>

        <p>
            ���û�ж�Ӧ�����������������Ǿ�ֱ�ӷ��ء�404������
        </p>

        <p>
            ������ǽ�<em>requestHandler.js</em>�޸�Ϊ������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> exec </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"child_process"</span><span
                class="pun">).</span><span class="pln">exec</span><span class="pun">;</span><span
                class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; exec</span><span class="pun">(</span><span
                class="str">"ls -lah"</span><span class="pun">,</span><span class="pln"> </span><span class="kwd">function</span><span
                class="pln"> </span><span class="pun">(</span><span class="pln">error</span><span
                class="pun">,</span><span class="pln"> stdout</span><span class="pun">,</span><span
                class="pln"> stderr</span><span class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">stdout</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">});</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> upload</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello Upload"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>exports</span><span class="pun">.</span><span class="pln">start </span><span
                class="pun">=</span><span class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ���ǵĴ����������Ҫ����response������Ϊ�˶���������ֱ�ӵ���Ӧ��
        </p>

        <p>
            <em>start</em>���������<em>exec()</em>�������ص���������������Ӧ�Ĳ�������<em>upload</em>���������Ȼ�Ǽ򵥵Ļظ���Hello World����ֻ�������ʹ��<em>response</em>������ѡ�
        </p>

        <p>
            ��ʱ�ٴ���������Ӧ�ã�<em>node index.js</em>����һ�ж��Ṥ���ĺܺá�
        </p>

        <p>
            �����Ҫ֤��<em>/start</em>��������к�ʱ�Ĳ�������������<em>/upload</em>��������������Ӧ�Ļ������Խ�<em>requestHandlers.js</em>�޸�Ϊ������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> exec </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"child_process"</span><span
                class="pun">).</span><span class="pln">exec</span><span class="pun">;</span><span
                class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; exec</span><span class="pun">(</span><span
                class="str">"find /"</span><span class="pun">,</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">{</span><span class="pln"> timeout</span><span class="pun">:</span><span
                class="pln"> </span><span class="lit">10000</span><span class="pun">,</span><span
                class="pln"> maxBuffer</span><span class="pun">:</span><span class="pln"> </span><span
                class="lit">20000</span><span class="pun">*</span><span class="lit">1024</span><span
                class="pln"> </span><span class="pun">},</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">function</span><span class="pln"> </span><span class="pun">(</span><span
                class="pln">error</span><span class="pun">,</span><span class="pln"> stdout</span><span
                class="pun">,</span><span class="pln"> stderr</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">write</span><span class="pun">(</span><span
                class="pln">stdout</span><span class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">});</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span
                class="kwd">function</span><span class="pln"> upload</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello Upload"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>exports</span><span class="pun">.</span><span class="pln">start </span><span
                class="pun">=</span><span class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ����һ����������<a href="http://localhost:8888/start" rel="nofollow">http://localhost:8888/start</a>��ʱ�򣬻Ứ10���ӵ�ʱ������룬��������<a href="http://localhost:8888/upload" rel="nofollow">http://localhost:8888/upload</a>��ʱ�򣬻�������Ӧ����Ȼ���ʱ��/start��Ӧ���ڴ����С�
        </p>

        <a name="serving-something-useful"></a>

        <h3>�����õĳ���</h3>

        <p>
            ��ĿǰΪֹ�����������Ѿ��ܺ��ˣ����ǣ����ǵ�Ӧ��û��ʵ����;��
        </p>

        <p>
            ������������·���Լ�����������Ѿ�����ˣ����������ǰ��մ�ǰ����������վ��ӽ������û�ѡ��һ���ļ����ϴ����ļ���Ȼ����������п����ϴ����ļ��� Ϊ�˱��ּ򵥣����Ǽ����û�ֻ���ϴ�ͼƬ��Ȼ������Ӧ�ý���ͼƬ��ʾ��������С�
        </p>

        <p>
            �ã������һ������ʵ�֣����ڴ�ǰ�Ѿ���JavaScriptԭ���Լ����Ե������������������ˣ�������Ǽӿ���ٶȡ�
        </p>

        <p>
            Ҫʵ�ָù��ܣ���Ϊ���������� ���ȣ���������������δ���POST���󣨷��ļ��ϴ�����֮������ʹ��Node.js��һ�������ļ��ϴ����ⲿģ�顣֮���Բ�������ʵ�ַ�ʽ���������ɡ�
        </p>

        <p>
            ��һ��������Node.js�д��������POST������ԱȽϼ򵥣�����������л�����ѧ���ܶࡣ
            <br>
            �ڶ�����Node.js�������ļ��ϴ���multipart POST�����ǱȽϸ��ӵģ���<em>��</em>�ڱ���ķ��룬�������ʹ���ⲿģ��ȴ���ڱ�����������֮�ڡ�
        </p>

        <a name="handling-post-requests"></a>

        <h4>����POST����</h4>

        <p>
            ��������һ���򵥵����ӣ�������ʾһ���ı�����textarea�����û��������ݣ�Ȼ��ͨ��POST�����ύ������������󣬷��������ܵ�����ͨ������������������չʾ��������С�
        </p>
        
        <p>
            <em>/start</em>����������������ɴ��ı����ı�����ˣ����ǽ�<em>requestHandlers.js</em>�޸�Ϊ������ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> body </span><span class="pun">=</span><span class="pln"> </span><span class="str">'&lt;html&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;meta http-equiv="Content-Type" content="text/html; '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'charset=UTF-8" /&gt;'</span><span class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" method="post"&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;textarea name="text" rows="20" cols="60"&gt;&lt;/textarea&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="submit" value="Submit text" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/form&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/html&gt;'</span><span class="pun">;</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/html"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">body</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"Hello Upload"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>exports</span><span class="pun">.</span><span class="pln">start </span><span
                class="pun">=</span><span class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ���ˣ��������ǵ�Ӧ���Ѿ��������ˣ������Ի�����Ƚ���Webby Awards���ˣ�������������ע�����Ƚ����ɹ��������������ѧѧԺ�������ѡȫ�������վ�Ľ������μ���ϸ˵����ͨ����������з���<a href="http://localhost:8888/start" rel="nofollow">http://localhost:8888/start</a>�Ϳ��Կ����򵥵ı��ˣ�Ҫ�ǵ�����������Ŷ��
        </p>

        <p>
            ����ܻ�˵������ֱ�ӽ��Ӿ�Ԫ�ط�������������еķ�ʽ̫��ª�ˡ�˵��û�����ǣ��Ҳ������ڱ����н�������MVC֮���ģʽ����Ϊ��������˽�JavaScript����Node.js������˵û����ϵ��
        </p>

        <p>
            ���µ�ƪ����������̽��һ������Ȥ�����⣺ ���û��ύ��ʱ������<em>/upload</em>�����������POST��������⡣
        </p>

        <p>
            ���ڣ������Ѿ��������е�ר���ˣ�����Ȼ���뵽�����첽�ص���ʵ�ַ������ش���POST��������ݡ�
        </p>

        <p>
            ������÷�������ʽ���������ǵģ���ΪPOST����һ�㶼�Ƚϡ��ء� ���� �û����ܻ�������������ݡ��������ķ�ʽ������������������Ȼ�ᵼ���û�������������
        </p>

        <p>
            Ϊ��ʹ�������̷�������Node.js�ὫPOST���ݲ�ֳɺܶ�С�����ݿ飬Ȼ��ͨ�������ض����¼�������ЩС���ݿ鴫�ݸ��ص�������������ض����¼���<em>data</em>�¼�����ʾ�µ�С���ݿ鵽���ˣ��Լ�<em>end</em>�¼�����ʾ���е����ݶ��Ѿ�������ϣ���
        </p>

        <p>
            ������Ҫ����Node.js����Щ�¼�������ʱ�򣬻ص���Щ��������ô�����أ� ����ͨ����<em>request</em>������ע��<em>������</em>��listener�� ��ʵ�֡������request������ÿ�ν��յ�HTTP����ʱ�򣬶���Ѹö��󴫵ݸ�<em>onRequest</em>�ص�������
        </p>

        <p>
            ������ʾ��
        </p>
        <pre class="prettyprint lang-js"><span class="pln">request</span><span class="pun">.</span><span class="pln">addListener</span><span
                class="pun">(</span><span class="str">"data"</span><span class="pun">,</span><span
                class="pln"> </span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">chunk</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; </span><span class="com">// called when a new chunk of data was received</span><span
                class="pln"><br></span><span class="pun">});</span><span class="pln"><br><br>request</span><span
                class="pun">.</span><span class="pln">addListener</span><span class="pun">(</span><span class="str">"end"</span><span
                class="pun">,</span><span class="pln"> </span><span class="kwd">function</span><span
                class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; </span><span
                class="com">// called when all chunks of data have been received</span><span
                class="pln"><br></span><span class="pun">});</span></pre>

        <p>
            �������ˣ��ⲿ���߼�д�������أ� ��������ֻ���ڷ������л�ȡ����<em>request</em>���� ���� ���ǲ�û����֮ǰ<em>response</em>������������ request ���󴫵ݸ�����·�ɺ����������
        </p>

        <p>
            ���ҿ�������ȡ����������������ݣ�Ȼ����Щ���ݸ�Ӧ�ò㴦��Ӧ����HTTP������Ҫ�������顣��ˣ��ҽ��飬����ֱ���ڷ������д���POST���ݣ�Ȼ�����յ����ݴ��ݸ�����·�ɺ����������������������н�һ���Ĵ���
        </p>

        <p>
            ��ˣ�ʵ��˼·���ǣ� ��<em>data</em>��<em>end</em>�¼��Ļص�����ֱ�ӷ��ڷ������У���<em>data</em>�¼��ص����ռ����е�POST���ݣ������յ��������ݣ�����<em>end</em>�¼�����ص�������������·�ɣ��������ݴ��ݸ�����Ȼ������·���ٽ������ݴ��ݸ����������
        </p>

        <p>
            ����ʲô��������ʵ�֡��ȴ�<em>server.js</em>��ʼ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; </span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> postData </span><span class="pun">=</span><span
                class="pln"> </span><span class="str">""</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; &nbsp; request</span><span
                class="pun">.</span><span class="pln">setEncoding</span><span class="pun">(</span><span class="str">"utf8"</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; &nbsp; request</span><span
                class="pun">.</span><span class="pln">addListener</span><span class="pun">(</span><span class="str">"data"</span><span
                class="pun">,</span><span class="pln"> </span><span class="kwd">function</span><span
                class="pun">(</span><span class="pln">postDataChunk</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; postData </span><span class="pun">+=</span><span class="pln"> postDataChunk</span><span
                class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Received POST data chunk '"</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; postDataChunk </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">"'."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="pun">});</span><span
                class="pln"><br><br>&nbsp; &nbsp; request</span><span class="pun">.</span><span
                class="pln">addListener</span><span class="pun">(</span><span class="str">"end"</span><span class="pun">,</span><span
                class="pln"> </span><span class="kwd">function</span><span class="pun">()</span><span
                class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; route</span><span class="pun">(</span><span
                class="pln">handle</span><span class="pun">,</span><span class="pln"> pathname</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">,</span><span class="pln"> postData</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="pun">});</span><span
                class="pln"><br><br>&nbsp; </span><span class="pun">}</span><span class="pln"><br><br>&nbsp; http</span><span
                class="pun">.</span><span class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>
            �������������������飺 ���ȣ����������˽������ݵı����ʽΪUTF-8��Ȼ��ע���ˡ�data���¼��ļ������������ռ�ÿ�ν��յ��������ݿ飬�����丳ֵ��<em>postData</em> ������������ǽ�����·�ɵĵ����Ƶ�<em>end</em>�¼���������У���ȷ����ֻ�ᵱ�������ݽ�����Ϻ�Ŵ���������ֻ����һ�Ρ�����ͬʱ����POST���ݴ��ݸ�����·�ɣ���Ϊ��Щ���ݣ������������õ���
        </p>

        <p>
            ����������ÿ�����ݿ鵽���ʱ���������־���������������������˵���Ǻܲ��õģ����������ܻ�ܴ󣬻��ǵðɣ��������ǣ��ڿ����׶��Ǻ����õģ������������ǿ���������ʲô��
        </p>

        <p>
            �ҽ�����Գ����£�������ȥ����һС���ı����Լ�������ݣ���������ݵ�ʱ�򣬾ͻᷢ��<em>data</em>�¼��ᴥ����Ρ�
        </p>

        <p>
            �������ġ����ǽ�������/uploadҳ�棬չʾ�û���������ݡ�Ҫʵ�ָù��ܣ�������Ҫ��<em>postData</em>���ݸ�����������޸�<em>router.js</em>Ϊ������ʽ��
        </p>

        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> route</span><span
                class="pun">(</span><span class="pln">handle</span><span class="pun">,</span><span
                class="pln"> pathname</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"About to route a request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">if</span><span
                class="pln"> </span><span class="pun">(</span><span class="kwd">typeof</span><span
                class="pln"> handle</span><span class="pun">[</span><span class="pln">pathname</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">===</span><span
                class="pln"> </span><span class="str">'function'</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; handle</span><span
                class="pun">[</span><span class="pln">pathname</span><span class="pun">](</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">);</span><span class="pln"><br>&nbsp; </span><span
                class="pun">}</span><span class="pln"> </span><span class="kwd">else</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"No request handler found for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">404</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"404 Not found"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">route </span><span class="pun">=</span><span
                class="pln"> route</span><span class="pun">;</span></pre>

        <p>
            Ȼ����<em>requestHandlers.js</em>�У����ǽ����ݰ����ڶ�<em>upload</em>�������Ӧ�У�
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> start</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">,</span><span class="pln"> postData</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> body </span><span class="pun">=</span><span class="pln"> </span><span class="str">'&lt;html&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;meta http-equiv="Content-Type" content="text/html; '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'charset=UTF-8" /&gt;'</span><span class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" method="post"&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;textarea name="text" rows="20" cols="60"&gt;&lt;/textarea&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="submit" value="Submit text" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/form&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/html&gt;'</span><span class="pun">;</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/html"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">body</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">,</span><span class="pln"> postData</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"You've sent: "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> postData</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br>exports</span><span class="pun">.</span><span class="pln">start </span><span
                class="pun">=</span><span class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ���ˣ��������ڿ��Խ���POST���ݲ�������������д���������ˡ�
        </p>

        <p>
            �������Ҫ�����ǣ� ��ǰ�����ǰ������������Ϣ�崫�ݸ�������·�ɺ��������������Ӧ��ֻ��POST�����У����Ǹ���Ȥ�Ĳ��ִ��ݸ�����·�ɺ������������������������У����Ǹ���Ȥ����ʵֻ��<em>text</em>�ֶΡ�
        </p>

        <p>
            ���ǿ���ʹ�ô�ǰ���ܹ���<em>querystring</em>ģ����ʵ�֣�
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> querystring </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"querystring"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> body </span><span class="pun">=</span><span class="pln"> </span><span class="str">'&lt;html&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;meta http-equiv="Content-Type" content="text/html; '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'charset=UTF-8" /&gt;'</span><span class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" method="post"&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;textarea name="text" rows="20" cols="60"&gt;&lt;/textarea&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="submit" value="Submit text" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/form&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/html&gt;'</span><span class="pun">;</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/html"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">body</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">,</span><span class="pln"> postData</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"You've sent the text: "</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; querystring</span><span class="pun">.</span><span
                class="pln">parse</span><span class="pun">(</span><span class="pln">postData</span><span
                class="pun">).</span><span class="pln">text</span><span class="pun">);</span><span class="pln"><br>&nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span></pre>

        <p>
            ���ˣ����Ͼ��ǹ��ڴ���POST���ݵ�ȫ�����ݡ�
        </p>

        <a name="handling-file-uploads"></a>

        <h4>�����ļ��ϴ�</h4>

        <p>
            ���������ʵ���������յ������������û��ϴ�ͼƬ��������ͼƬ�����������ʾ������
        </p>

        <p>
            �ص�90��������������ȫ������������IPO����ҵģ���ˣ��������ͨ������ѧ�������������飺 ��ΰ�װ�ⲿNode.jsģ�飬�Լ���ν�����Ӧ�õ����ǵ�Ӧ���С�
        </p>

        <p>
            ��������Ҫ�õ����ⲿģ����Felix Geisend?rfer������<em>node-formidable</em>ģ�顣���Խ����ϴ����ļ��������˺ܺõĳ��� ��ʵ˵���ˣ������ļ��ϴ�<em>�����ǡ�</em>����POST���� ���� ���ǣ��鷳�����ھ���Ĵ���ϸ�ڣ����ԣ���������ֳɵķ��������ʵ㡣
        </p>

        <p>
            ʹ�ø�ģ�飬������Ҫ��װ��ģ�顣Node.js�����Լ��İ�����������<em>NPM</em>���������ð�װNode.js���ⲿģ���÷ǳ����㡣ͨ������һ������Ϳ�����ɸ�ģ��İ�װ��
        </p>
        <pre class="prettyprint lang-bash"><span class="pln">npm install formidable</span></pre>

        <p>
            ����ն�����������ݣ�
        </p>
        <pre class="prettyprint lang-bash"><span class="pln">npm info build </span><span class="typ">Success</span><span
                class="pun">:</span><span class="pln"> formidable@1</span><span class="pun">.</span><span class="lit">0.9</span><span
                class="pln"><br>npm ok</span></pre>

        <p>
            ��˵��ģ���Ѿ���װ�ɹ��ˡ�
        </p>

        <p>
            �������ǾͿ�����<em>formidable</em>ģ���ˡ���ʹ���ⲿģ�����ڲ�ģ�����ƣ���require��佫�����뼴�ɣ�
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> formidable </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"formidable"</span><span
                class="pun">);</span></pre>

        <p>
            �����ģ�����ľ��ǽ�ͨ��HTTP POST�����ύ�ı�����Node.js�п��Ա�����������Ҫ���ľ��Ǵ���һ���µ�<em>IncomingForm</em>�����Ƕ��ύ���ĳ����ʾ��֮�󣬾Ϳ�����������request���󣬻�ȡ������Ҫ�������ֶΡ�
        </p>

        <p>
            node-formidable�ٷ�������չʾ����������������ں���һ�����ģ�
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> formidable </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">'formidable'</span><span
                class="pun">),</span><span class="pln"><br>&nbsp; &nbsp; http </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">'http'</span><span
                class="pun">),</span><span class="pln"><br>&nbsp; &nbsp; sys </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">'sys'</span><span
                class="pun">);</span><span class="pln"><br><br>http</span><span class="pun">.</span><span class="pln">createServer</span><span
                class="pun">(</span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">req</span><span class="pun">,</span><span class="pln"> res</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span
                class="pln"><br>&nbsp; </span><span class="kwd">if</span><span class="pln"> </span><span
                class="pun">(</span><span class="pln">req</span><span class="pun">.</span><span
                class="pln">url </span><span class="pun">==</span><span class="pln"> </span><span
                class="str">'/upload'</span><span class="pln"> </span><span class="pun">&amp;&amp;</span><span
                class="pln"> req</span><span class="pun">.</span><span class="pln">method</span><span
                class="pun">.</span><span class="pln">toLowerCase</span><span class="pun">()</span><span
                class="pln"> </span><span class="pun">==</span><span class="pln"> </span><span class="str">'post'</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="com">// parse a file upload</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="kwd">var</span><span
                class="pln"> form </span><span class="pun">=</span><span class="pln"> </span><span
                class="kwd">new</span><span class="pln"> formidable</span><span class="pun">.</span><span class="typ">IncomingForm</span><span
                class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; form</span><span class="pun">.</span><span
                class="pln">parse</span><span class="pun">(</span><span class="pln">req</span><span class="pun">,</span><span
                class="pln"> </span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">err</span><span class="pun">,</span><span class="pln"> fields</span><span
                class="pun">,</span><span class="pln"> files</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; res</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">'content-type'</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">'text/plain'</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; res</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">'received upload:\n\n'</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; res</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">(</span><span
                class="pln">sys</span><span class="pun">.</span><span class="pln">inspect</span><span
                class="pun">({</span><span class="pln">fields</span><span class="pun">:</span><span
                class="pln"> fields</span><span class="pun">,</span><span class="pln"> files</span><span
                class="pun">:</span><span class="pln"> files</span><span class="pun">}));</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="kwd">return</span><span
                class="pun">;</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span class="pln"><br><br>&nbsp; </span><span
                class="com">// show a file upload form</span><span class="pln"><br>&nbsp; res</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">'content-type'</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">'text/html'</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; res</span><span class="pun">.</span><span class="pln">end</span><span
                class="pun">(</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" enctype="multipart/form-data" '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'method="post"&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="text" name="title"&gt;&lt;br&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="file" name="upload" multiple="multiple"&gt;&lt;br&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="submit" value="Upload"&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/form&gt;'</span><span class="pln"><br>&nbsp; </span><span class="pun">);</span><span
                class="pln"><br></span><span class="pun">}).</span><span class="pln">listen</span><span
                class="pun">(</span><span class="lit">8888</span><span class="pun">);</span></pre>

        <p>
            ������ǽ��������룬���浽һ���ļ��У���ͨ��<em>node</em>��ִ�У��Ϳ��Խ��м򵥵ı��ύ�ˣ������ļ��ϴ���Ȼ�󣬿��Կ���ͨ������<em>form.parse</em>���ݸ��ص�������<em>files</em>��������ݣ�������ʾ��
        </p>
        <pre class="lang-js">received upload:

{ fields: { title: 'Hello World' },
  files:
   { upload:
      { size: 1558,
        path: '/tmp/1c747974a27a6292743669e91f29350b',
        name: 'us-flag.png',
        type: 'image/png',
        lastModifiedDate: Tue, 21 Jun 2011 07:02:41 GMT,
        _writeStream: [Object],
        length: [Getter],
        filename: [Getter],
        mime: [Getter] } } }</pre>

        <p>
            Ϊ��ʵ�����ǵĹ��ܣ�������Ҫ����������Ӧ�õ����ǵ�Ӧ���У����⣬���ǻ�Ҫ������ν��ϴ��ļ������ݣ�������<em>/tmp</em>Ŀ¼�У���ʾ��������С�
        </p>

        <p>
            ����������������Ǹ����⣺ ���ڱ����ڱ���Ӳ���е��ļ�����β�����������п����أ�
        </p>

        <p>
            ��Ȼ��������Ҫ�����ļ���ȡ�����ǵķ������У�ʹ��һ����<em>fs</em>��ģ�顣
        </p>

        <p>
            ���������<em>/show</em>URL����������򣬸ô������ֱ��Ӳ���뽫�ļ�<em>/tmp/test.png</em>����չʾ��������С���Ȼ�ˣ�������Ҫ����ͼƬ���浽���λ�ò��С�
        </p>

        <p>
            ��<em>requestHandlers.js</em>�޸�Ϊ������ʽ��
        </p>

        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> querystring </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"querystring"</span><span
                class="pun">),</span><span class="pln"><br>&nbsp; &nbsp; fs </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"fs"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> body </span><span class="pun">=</span><span class="pln"> </span><span class="str">'&lt;html&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;meta http-equiv="Content-Type" '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'content="text/html; charset=UTF-8" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" method="post"&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;textarea name="text" rows="20" cols="60"&gt;&lt;/textarea&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="submit" value="Submit text" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/form&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/html&gt;'</span><span class="pun">;</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/html"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">body</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">,</span><span class="pln"> postData</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"You've sent the text: "</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; querystring</span><span class="pun">.</span><span
                class="pln">parse</span><span class="pun">(</span><span class="pln">postData</span><span
                class="pun">).</span><span class="pln">text</span><span class="pun">);</span><span class="pln"><br>&nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> show</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'show' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; fs</span><span class="pun">.</span><span class="pln">readFile</span><span
                class="pun">(</span><span class="str">"/tmp/test.png"</span><span class="pun">,</span><span
                class="pln"> </span><span class="str">"binary"</span><span class="pun">,</span><span
                class="pln"> </span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">error</span><span class="pun">,</span><span class="pln"> file</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">if</span><span class="pun">(</span><span class="pln">error</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">500</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">error </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">"\n"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">}</span><span class="pln"> </span><span class="kwd">else</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"image/png"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">file</span><span
                class="pun">,</span><span class="pln"> </span><span class="str">"binary"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">}</span><span class="pln"><br>&nbsp; </span><span class="pun">});</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">show </span><span class="pun">=</span><span
                class="pln"> show</span><span class="pun">;</span></pre>

        <p>
            ���ǻ���Ҫ�����µ������������ӵ�<em>index.js</em>�е�·��ӳ����У�
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> server </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"./server"</span><span
                class="pun">);</span><span class="pln"><br></span><span class="kwd">var</span><span
                class="pln"> router </span><span class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"./router"</span><span class="pun">);</span><span class="pln"><br></span><span class="kwd">var</span><span
                class="pln"> requestHandlers </span><span class="pun">=</span><span class="pln"> require</span><span
                class="pun">(</span><span class="str">"./requestHandlers"</span><span class="pun">);</span><span
                class="pln"><br><br></span><span class="kwd">var</span><span class="pln"> handle </span><span
                class="pun">=</span><span class="pln"> </span><span class="pun">{}</span><span
                class="pln"><br>handle</span><span class="pun">[</span><span class="str">"/"</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">=</span><span class="pln"> requestHandlers</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">;</span><span class="pln"><br>handle</span><span
                class="pun">[</span><span class="str">"/start"</span><span class="pun">]</span><span
                class="pln"> </span><span class="pun">=</span><span class="pln"> requestHandlers</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">;</span><span class="pln"><br>handle</span><span
                class="pun">[</span><span class="str">"/upload"</span><span class="pun">]</span><span
                class="pln"> </span><span class="pun">=</span><span class="pln"> requestHandlers</span><span
                class="pun">.</span><span class="pln">upload</span><span class="pun">;</span><span class="pln"><br>handle</span><span
                class="pun">[</span><span class="str">"/show"</span><span class="pun">]</span><span class="pln"> </span><span
                class="pun">=</span><span class="pln"> requestHandlers</span><span class="pun">.</span><span
                class="pln">show</span><span class="pun">;</span><span class="pln"><br><br>server</span><span
                class="pun">.</span><span class="pln">start</span><span class="pun">(</span><span
                class="pln">router</span><span class="pun">.</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">);</span></pre>

        <p>
            ����������֮��ͨ������<a href="http://localhost:8888/show" rel="nofollow">http://localhost:8888/show</a>���Ϳ��Կ���������<em>/tmp/test.png</em>��ͼƬ�ˡ�
        </p>

        <p>
            �ã��������Ҫ�ľ��ǣ�
        </p>
        
        <p>
            <ul>
                <li>
                    ��<em>/start</em>�������һ���ļ��ϴ�Ԫ��
                </li>
                <li>
                    ��node-formidable���ϵ����ǵ�<em>upload</em>����������У����ڽ��ϴ���ͼƬ���浽<em>/tmp/test.png</em>
                </li>
        
                <li>
                    ���ϴ���ͼƬ��Ƕ��<em>/upload</em>URL�����HTML��
                </li>
            </ul>
        </p>

        <p>
            ��һ��ܼ򵥡�ֻ��Ҫ��HTML���У����һ��<em>multipart/form-data</em>�ı������ͣ��Ƴ���ǰ���ı��������һ���ļ��ϴ�����������ύ��ť���İ���Ϊ��Upload file�����ɡ� ����<em>requestHandler.js</em>��ʾ��
        </p>

        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> querystring </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"querystring"</span><span
                class="pun">),</span><span class="pln"><br>&nbsp; &nbsp; fs </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"fs"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> body </span><span class="pun">=</span><span class="pln"> </span><span class="str">'&lt;html&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;meta http-equiv="Content-Type" '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'content="text/html; charset=UTF-8" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" enctype="multipart/form-data" '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'method="post"&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;input type="file" name="upload"&gt;'</span><span class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;input type="submit" value="Upload file" /&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/form&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/body&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/html&gt;'</span><span
                class="pun">;</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/html"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">body</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">,</span><span class="pln"> postData</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/plain"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"You've sent the text: "</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; querystring</span><span class="pun">.</span><span
                class="pln">parse</span><span class="pun">(</span><span class="pln">postData</span><span
                class="pun">).</span><span class="pln">text</span><span class="pun">);</span><span class="pln"><br>&nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> show</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> postData</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'show' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; fs</span><span class="pun">.</span><span class="pln">readFile</span><span
                class="pun">(</span><span class="str">"/tmp/test.png"</span><span class="pun">,</span><span
                class="pln"> </span><span class="str">"binary"</span><span class="pun">,</span><span
                class="pln"> </span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">error</span><span class="pun">,</span><span class="pln"> file</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">if</span><span class="pun">(</span><span class="pln">error</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">500</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">error </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">"\n"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">}</span><span class="pln"> </span><span class="kwd">else</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"image/png"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">file</span><span
                class="pun">,</span><span class="pln"> </span><span class="str">"binary"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">}</span><span class="pln"><br>&nbsp; </span><span class="pun">});</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">show </span><span class="pun">=</span><span
                class="pln"> show</span><span class="pun">;</span></pre>

        <p>
            �ܺá���һ����ԱȽϸ��ӡ�����������һ�����⣺ ������Ҫ��<em>upload</em>��������ж��ϴ����ļ����д��������Ļ������Ǿ���Ҫ��<em>request</em>���󴫵ݸ�node-formidable��<em>form.parse</em>������
        </p>

        <p>
            ���ǣ������е�ֻ��<em>response</em>�����<em>postData</em>���顣�����ӣ�����ֻ�ܲ��ò���<em>request</em>����ӷ�������ʼһ·ͨ������·�ɣ��ٴ��ݸ���������� �����и��õķ��������ǣ�������ô˵��Ŀǰ�����������������ǵ�����
        </p>

        <p>
            ��������ǿ��Խ�<em>postData</em>�ӷ������Լ�������������Ƴ��� ���� һ���棬�������Ǵ����ļ��ϴ���˵�Ѿ�����Ҫ�ˣ�����һ���棬���������ܻ���������һ�����⣺ �����Ѿ������ġ���<em>request</em>�����е����ݣ�����ζ�ţ�����<em>form.parse</em>��˵��������Ҫ��ȡ���ݵ�ʱ���ʲôҲ��ȡ�����ˡ�����ΪNode.js��������������棩
        </p>

        <p>
            ���Ǵ�<em>server.js</em>��ʼ ���� �Ƴ���postData�Ĵ����Լ�<em>request.setEncoding</em>
            ���ⲿ��node-formidable����ᴦ����ת�����ý�<em>request</em>���󴫵ݸ�����·�ɵķ�ʽ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> http </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span
                class="str">"http"</span><span class="pun">);</span><span class="pln"><br></span><span
                class="kwd">var</span><span class="pln"> url </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"url"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">route</span><span
                class="pun">,</span><span class="pln"> handle</span><span class="pun">)</span><span class="pln"> </span><span
                class="pun">{</span><span class="pln"><br>&nbsp; </span><span class="kwd">function</span><span
                class="pln"> onRequest</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">var</span><span class="pln"> pathname </span><span class="pun">=</span><span class="pln"> url</span><span
                class="pun">.</span><span class="pln">parse</span><span class="pun">(</span><span
                class="pln">request</span><span class="pun">.</span><span class="pln">url</span><span
                class="pun">).</span><span class="pln">pathname</span><span class="pun">;</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">" received."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; route</span><span class="pun">(</span><span
                class="pln">handle</span><span class="pun">,</span><span class="pln"> pathname</span><span
                class="pun">,</span><span class="pln"> response</span><span class="pun">,</span><span class="pln"> request</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br><br>&nbsp; http</span><span class="pun">.</span><span
                class="pln">createServer</span><span class="pun">(</span><span class="pln">onRequest</span><span
                class="pun">).</span><span class="pln">listen</span><span class="pun">(</span><span
                class="lit">8888</span><span class="pun">);</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Server has started."</span><span
                class="pun">);</span><span class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span></pre>

        <p>
            �������� router.js ���� ���ǲ�����Ҫ����<em>postData</em>�ˣ����Ҫ����<em>request</em>����
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">function</span><span class="pln"> route</span><span
                class="pun">(</span><span class="pln">handle</span><span class="pun">,</span><span
                class="pln"> pathname</span><span class="pun">,</span><span class="pln"> response</span><span
                class="pun">,</span><span class="pln"> request</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"About to route a request for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; </span><span class="kwd">if</span><span
                class="pln"> </span><span class="pun">(</span><span class="kwd">typeof</span><span
                class="pln"> handle</span><span class="pun">[</span><span class="pln">pathname</span><span
                class="pun">]</span><span class="pln"> </span><span class="pun">===</span><span
                class="pln"> </span><span class="str">'function'</span><span class="pun">)</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; handle</span><span
                class="pun">[</span><span class="pln">pathname</span><span class="pun">](</span><span class="pln">response</span><span
                class="pun">,</span><span class="pln"> request</span><span class="pun">);</span><span class="pln"><br>&nbsp; </span><span
                class="pun">}</span><span class="pln"> </span><span class="kwd">else</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"No request handler found for "</span><span
                class="pln"> </span><span class="pun">+</span><span class="pln"> pathname</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">404</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/html"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="str">"404 Not found"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">}</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">route </span><span class="pun">=</span><span
                class="pln"> route</span><span class="pun">;</span></pre>

        <p>
            ���ڣ�<em>request</em>����Ϳ��������ǵ�<em>upload</em>�����������ʹ���ˡ�node-formidable�ᴦ���ϴ����ļ����浽����<em>/tmp</em>Ŀ¼�У���������Ҫ������ȷ�����ļ������<em>/tmp/test.png</em>�� û�����Ǳ��ּ򵥣�������ֻ�����ϴ�PNGͼƬ��
        </p>

        <p>
            �������<em>fs.renameSync(path1,path2)</em>��ʵ�֡�Ҫע����ǣ������������÷�����ͬ��ִ�еģ�
            Ҳ����˵��������������Ĳ����ܺ�ʱ�Ļ��������� ��������Ȳ����ǡ�
        </p>

        <p>
            �����������ǰѴ����ļ��ϴ��Լ��������Ĳ����ŵ�һ������<em>requestHandlers.js</em>��ʾ��
        </p>
        <pre class="prettyprint lang-js"><span class="kwd">var</span><span class="pln"> querystring </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"querystring"</span><span
                class="pun">),</span><span class="pln"><br>&nbsp; &nbsp; fs </span><span class="pun">=</span><span
                class="pln"> require</span><span class="pun">(</span><span class="str">"fs"</span><span
                class="pun">),</span><span class="pln"><br>&nbsp; &nbsp; formidable </span><span
                class="pun">=</span><span class="pln"> require</span><span class="pun">(</span><span class="str">"formidable"</span><span
                class="pun">);</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> start</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'start' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> body </span><span class="pun">=</span><span class="pln"> </span><span class="str">'&lt;html&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;meta http-equiv="Content-Type" content="text/html; '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'charset=UTF-8" /&gt;'</span><span class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/head&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;form action="/upload" enctype="multipart/form-data" '</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'method="post"&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="file" name="upload" multiple="multiple"&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;input type="submit" value="Upload file" /&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/form&gt;'</span><span class="pun">+</span><span
                class="pln"><br>&nbsp; &nbsp; </span><span class="str">'&lt;/body&gt;'</span><span
                class="pun">+</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="str">'&lt;/html&gt;'</span><span class="pun">;</span><span class="pln"><br><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/html"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">body</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br></span><span
                class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span class="pln"> upload</span><span
                class="pun">(</span><span class="pln">response</span><span class="pun">,</span><span class="pln"> request</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'upload' was called."</span><span
                class="pun">);</span><span class="pln"><br><br>&nbsp; </span><span class="kwd">var</span><span
                class="pln"> form </span><span class="pun">=</span><span class="pln"> </span><span
                class="kwd">new</span><span class="pln"> formidable</span><span class="pun">.</span><span class="typ">IncomingForm</span><span
                class="pun">();</span><span class="pln"><br>&nbsp; console</span><span class="pun">.</span><span
                class="pln">log</span><span class="pun">(</span><span class="str">"about to parse"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; form</span><span class="pun">.</span><span
                class="pln">parse</span><span class="pun">(</span><span class="pln">request</span><span
                class="pun">,</span><span class="pln"> </span><span class="kwd">function</span><span
                class="pun">(</span><span class="pln">error</span><span class="pun">,</span><span
                class="pln"> fields</span><span class="pun">,</span><span class="pln"> files</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"parsing done"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; fs</span><span class="pun">.</span><span
                class="pln">renameSync</span><span class="pun">(</span><span class="pln">files</span><span
                class="pun">.</span><span class="pln">upload</span><span class="pun">.</span><span
                class="pln">path</span><span class="pun">,</span><span class="pln"> </span><span class="str">"/tmp/test.png"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">writeHead</span><span class="pun">(</span><span class="lit">200</span><span
                class="pun">,</span><span class="pln"> </span><span class="pun">{</span><span
                class="str">"Content-Type"</span><span class="pun">:</span><span class="pln"> </span><span class="str">"text/html"</span><span
                class="pun">});</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span
                class="str">"received image:&lt;br/&gt;"</span><span class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">write</span><span class="pun">(</span><span class="str">"&lt;img src='/show' /&gt;"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; </span><span class="pun">});</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br></span><span class="kwd">function</span><span
                class="pln"> show</span><span class="pun">(</span><span class="pln">response</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; console</span><span
                class="pun">.</span><span class="pln">log</span><span class="pun">(</span><span class="str">"Request handler 'show' was called."</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; fs</span><span class="pun">.</span><span class="pln">readFile</span><span
                class="pun">(</span><span class="str">"/tmp/test.png"</span><span class="pun">,</span><span
                class="pln"> </span><span class="str">"binary"</span><span class="pun">,</span><span
                class="pln"> </span><span class="kwd">function</span><span class="pun">(</span><span
                class="pln">error</span><span class="pun">,</span><span class="pln"> file</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="kwd">if</span><span class="pun">(</span><span class="pln">error</span><span
                class="pun">)</span><span class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">500</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"text/plain"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">error </span><span
                class="pun">+</span><span class="pln"> </span><span class="str">"\n"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">}</span><span class="pln"> </span><span class="kwd">else</span><span
                class="pln"> </span><span class="pun">{</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">writeHead</span><span class="pun">(</span><span
                class="lit">200</span><span class="pun">,</span><span class="pln"> </span><span
                class="pun">{</span><span class="str">"Content-Type"</span><span class="pun">:</span><span
                class="pln"> </span><span class="str">"image/png"</span><span class="pun">});</span><span
                class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span class="pun">.</span><span
                class="pln">write</span><span class="pun">(</span><span class="pln">file</span><span
                class="pun">,</span><span class="pln"> </span><span class="str">"binary"</span><span
                class="pun">);</span><span class="pln"><br>&nbsp; &nbsp; &nbsp; response</span><span
                class="pun">.</span><span class="pln">end</span><span class="pun">();</span><span class="pln"><br>&nbsp; &nbsp; </span><span
                class="pun">}</span><span class="pln"><br>&nbsp; </span><span class="pun">});</span><span
                class="pln"><br></span><span class="pun">}</span><span class="pln"><br><br>exports</span><span
                class="pun">.</span><span class="pln">start </span><span class="pun">=</span><span
                class="pln"> start</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">upload </span><span class="pun">=</span><span
                class="pln"> upload</span><span class="pun">;</span><span class="pln"><br>exports</span><span
                class="pun">.</span><span class="pln">show </span><span class="pun">=</span><span
                class="pln"> show</span><span class="pun">;</span></pre>

        <p>
            ���ˣ�����������������Ӧ�����еĹ��ܾͿ������ˡ�ѡ��һ�ű���ͼƬ�������ϴ�����������Ȼ��������ͻ���ʾ��ͼƬ��
        </p>

        <a name="conclusion-and-outlook"></a>

        <h2>�ܽ���չ��</h2>

        <p>
            ��ϲ�����ǵ������Ѿ�����ˣ����ǿ�������һ��Node.js��webӦ�ã�Ӧ����С����ȴ�������ȫ���� �ڼ䣬���ǽ����˺ܶ༼���㣺�����JavaScript������ʽ��̡���������������ص����¼����ڲ����ⲿģ��ȵȡ�
        </p>

        <p>
            ��Ȼ�ˣ�������౾��û�н��ܵ��ģ� ��β������ݿ⡢��ν��е�Ԫ���ԡ���ο���Node.js���ⲿģ���Լ�һЩ�򵥵�������λ�ȡGET����֮��ķ�����
        </p>

        <p>
            ������Ͼ�ֻ��һ������ѧ�ߵĽ̳� ���� �����ܸ��ǵ����е����ݡ�
        </p>

        <p>
            ���˵��ǣ�Node.js�����ǳ���Ծ��������ǡ���ı�����������һȺ�жද֢С������һ���ܲ���Ծ�𣿣���
            ����ζ�ţ���������Node.js����Դ����ʲô���ⶼ����������Ѱ����
            ����<a href="https://github.com/joyent/node/wiki">Node.js������wiki</a>�Լ�
            <a href="http://www.nodecloud.org/">NodeCloud</a>������õ���Դ��
        </p>
        </div>


        <div id="footer">
            <p id="ccimage">
                <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/"><img alt="Creative Commons License" border="0" src="creative_commons.png" width="88" height="31"/></a>
            </p>
            <p>
                <span xmlns:dct="http://purl.org/dc/terms/">The Node Beginner Book</span>
                by
                <a xmlns:cc="http://creativecommons.org/ns#" href="http://manuel.kiessling.net" rel="cc:attributionURL">Manuel Kiessling</a> (see <a href="https://plus.google.com/100272082905360445612?rel=author">Google+ profile</a>)
                is licensed under a
                <br />
                <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/">Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License</a>.
                <br />
                Permissions beyond the scope of this license may be available at <a xmlns:cc="http://creativecommons.org/ns#" href="mailto:manuel@kiessling.net" rel="cc:morePermissions">manuel@kiessling.net</a>.
            </p>
        </div>