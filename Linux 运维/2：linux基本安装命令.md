### Linux ���ǻ���Unix�Ŀ�Դ��ѵĲ���ϵͳ������ϵͳ���ȶ��ԺͰ�ȫ�Լ�����Ϊ����Ĵ������е����ϵͳ����

###### ���ࣺ

1��ͼ�λ������
2���������棺�����н���

###### ����ԭ���̶�

1���ں˰汾��linus�쵼���ں�С�鿪����ά����
2�����а汾����������˾���ο������·��У�ubuntu��CentOS��redhat

### 1��������

  Ctrl+alt+F2  : ��������
  Ctrl+alt+F1  : �ر�������

### 2����¼

root��Ȩ�޴����벻����
shutdown now   �ػ�	

reboot  ����

ctrl+l   ����

### 3��init 3 �л��������У����µ�¼

?      init 5 �л���GUI��¼����

### 4��Ctrl+L ����

?     exit :�˳�������ϵͳ

### 5��ping ip��ַ  ��������Ƿ���ͨ

?      ping ����   

### 6��ip addr �鿴����

### 7����������

   cd /   ��....

   ����������
   cd /etc/sysconfig/network-scripts   
   ls  : �鿴��ǰ�ļ���
	��ɫ�ģ���ʾĿ¼
        ��ɫ�ģ���ʾѹ���ļ�
	��ɫ�ģ���ʾ��ͨ�ļ�
	��ɫ�ģ���ʾ��ִ���ļ�

   �鿴�������ƣ�����༭��
   vi ifcfg-ens33

   ����༭��ģʽ
   ��ONBOOT=NO�޸�Ϊyes������i���������ģʽ��������ģʽ��

   ����:wq ��س�(�����˳��༭��)
   service network restart   :�����������
   ping ����    ---------��������Ƿ�ƴͨ

### 8��yumԴ�滻��Linuxϵͳ��װ���·����-------������ϵ

���׿�Ԫ������վ��http://mirrors.163.com
http://mirrors.163.com/.help/CentOS7-Base-163.repo   yumԴ����

��ñ(redHat)ϵ���У����������װ�ķ���
	

cd /etc/yum.repos.d   ��yumԴ�����ļ�·��

cd ..  ������һ��

rm -rf yum.repos.d    ɾ�� -ǿ��ɾ��  �ļ���

mkdir yum.repos.d     ����  �ļ���

cd /etc/yum.repos.d   �����Ŀ¼

wget http://mirrors.163.com/.help/CentOS7-Base-163.repo   �滻yumԴ

http://mirrors.aliyun.com/repo/Centos-7.repo           ���￪Դ����

yum clean all      ���yumԴ����

yum makecache        �������

yum repolist  all    ���yumԴ�����ļ��Ƿ�����

yum update kernel    �����ں�

yum update          �����������



### 9��	root�����޸�

1������ϵͳ reboot

2���������������¼����ٵ������E��

3�����������Ԯģʽ������ģʽ��

4����λLinux16 �����У��ҵ� ro ɾ����ԭλ����� rw init=/sysroot/bin/bash ֮��������  Ctrl+x

5������ chroot /sysroot

6: ���� passwd

7: �����������룬������

8��ʹ��������Ч�� touch /.autorelabel

9: �������Ctrl+d

10: ���룺reboot ����

### 10��   Զ�̵�¼��putty����XShell�����˿ںţ�`23`

Centos�����룺ip addr  �ڱ�������ens33�м�¼����IP��ַ
Windows��˫����putty���� Host name��IP addrs��������centos�е�IP��
��putty�е�Saved sessions ������������Ҳ�save����ַ���˿�Ϊ22����
���putty�²��open������Զ�̵�¼	
����root ����������



### ��ݼ�

tab����ȫ����
ctrl+C����ֹ��ǰ����
ctrl+D���˳���ǰ�ն�
ctrl+L������
ctrl+Z����ֹ����

ctrl+A��������ƶ�������
ctrl+E������ƶ��������












