# ��������java������ּ�<br><br>

## һ.ǰ��<br>
����Ŀ����webcollector������,ͨ����򵥵ķ�ʽ�ṩ��һ������������java���濪�����ּ�<br><br>

## ��.��Ŀ����<br>
<ul>
    <li>lombok</li>
    <li>slf4j-api</li>
    <li>log4j2</li>
    <li>okhttp(��ѡ)</li>
</ul>

## ��.ʹ��<br>
�Զ���````Requester````��````Visitor````�Ľӿ�ʵ����<br><br>
һ�����ٿ�ʼ������:<br>
````
    new Crawler()
        //ִ������ʵ��
        .requester(requester)
        //�������ʵ��
        .visitor(visitor)
        //ִ���߳���
        .thread(3)
        //������,����
        .requestInterval(200L)
        //�����������
        .add(new Seed("http://www.luoyifan.com"))
        //����
        .start();
````
��Ϊ���ٿ�ʼ�����ӵ�һ����,Ŀǰ��````extend````ģ�����ṩ��2��������ʵ����<br>
````OkHttpRequester````��````ConsoleVisitor````<br>
���Ƿֱ�ʵ����````Requester````�ӿں�````Visitor````�ӿ�<br>
��ʹ��OkHttpֱ�ӽ������󲢽����ؽ����ӡ�ڿ���̨��