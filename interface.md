# OSN-CONNECTOR �ӿ��ĵ�
IM�������¼��IMS������������OSN-connector(���¼��OSNC)�������ݽ�����
IMS��OSNC֮��ͨ��http����ͨ�ţ�ͨ�Ÿ�ʽΪjson��ʽ��

1. ������Ϣ  

��IMS������Ϣ����ʱ����ͨ��OSNC֪ͨ�Է�ȡ�����ݡ�
��������IMS���͸�OSNC�������͡�
```
{
command:message
to:[OSNID]
}
```

2. �����û�  

��OSNC���յ�����OSNC�Ĳ����û���Ϣʱ��֪ͨOSNC��
��������OSNC���͸�IMS�������͡�
```
{
command:finduser
hash:[OSNID��hash]
ip:[target ip]
}
```

3. ��ȡ��Ϣ��Դ�б�  

��IMS���յ�finduser�����ж�finduserΪ�Լ����û�ʱ��������Ϣ��ȡ��Ϣ��Դ�б�
��������IMS���͸�OSNC���Է�OSNC�յ��Ժ�Ҳ��ת����IMS��
```
{
command:getmsglist
hash:[OSNID��hash]
ip:[����finduser��ip]
}
```
IMS�ظ�
```
{
to:OSNID
from:[OSNID1,OSNID2,OSNID3...]
}
```

4. ��ȡ�û���Ϣ

��������IMS���͸�OSNC���Է�OSNC�յ��Ժ�Ҳ��ת����IMS��
```
{
command:getmsg
from:[OSNID��Դ��]
to:[OSNID���շ�]
ip:[target ip]
}
```
IMS�ظ�
```
{
[msg1,msg2,msg3...]
}
```

5. OSNIDתhash

��������IMS���͸�OSNC��
```
{
command:gethash
user:OSNID
}
```
OSNC�ظ���
```
{
errCode:0
hash:ipsf user hash
}
```
