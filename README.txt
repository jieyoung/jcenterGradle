5����ʹ��git
��װgit
����ssh��Կ��Ĭ�ϻ����û�~����Ŀ¼�������� id_rsa˽Կ, id_rsa.pub��Կ2���ļ���
$ ssh-keygen -t rsa -C "youremail@yourcompany.com"

#git����cmd
��ȡ�ֿ���� 
git clone <git��ַ>

git�ֿ��ʼ��
git init

��鵱ǰ�ļ�״̬
git status

�������ļ�/�ݴ����޸��ļ�
git add <�޸ĵ��ļ����ļ���> 

�ύgit add���ļ� 
git commit -m "<ע��>"

����ĳЩ�ļ�
�༭.gitignore

������֧ 
git checkout -b <branch>

�л���֧(������) 
git checkout <branch>

�����ش���ͬ����Զ�� 
git push origin <branch>

������branch1ͬ����Զ�˵�branch2 
git push origin <branch1>:<branch2>

ɾ��Զ�̷�֧, ���صĻ��ᱣ�� 
git push origin :<branch>

�ϲ������branch1��֧������branch2��֧�� ����г�ͻ�����ֶ��޸ĳ�ͻ���ύֱ��û�г�ͻ 
git pull origin <branch1>:<branch2>

��tag1 
git tag -a <tag1> -m "<ע��>"
git push origin --tags  
git tag -d <tagname>

ɾ��Զ�˷�֧
git push origin --delete <branchName>
���� ����һ���շ�֧��Զ�̷�֧����ʵ���൱��ɾ��Զ�̷�֧��
git push origin :<branchName>

ɾ�������ڶ�ӦԶ�̷�֧�ı��ط�֧
git fetch -p

��ȡԶ��tag
git fetch origin tag <tagname>

������Զ�̷�֧
��git��������Զ�̷�֧����ʵ������ɾ��Զ�̷�֧��Ȼ�����������ط�֧���������ύһ��Զ�̷�֧��
git branch -av  �鿴��Щ��֧
1��git push --delete origin devel  ɾ��Զ�̷�֧devel
2, git br -m devel develop  ���������ط�֧
3, git push origin develop ���ͱ��ط�֧

�鿴����Щtag
git tag -ln

git lg