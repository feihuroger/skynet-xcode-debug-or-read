һ��ֱ�� skynet �� ���� skynet.xcodeproj


�����Լ��������ذ�װ�����ù���

1.��ѹ ./skynet-1.0.0-alpha.zip �� ./skynet

2.��ѹ ./jemalloc-3.6.0.tar.bz2 �� ./skynet/3rd/jemalloc/

3.���� jemalloc
   cd �� jemalloc Ŀ¼��
   ./configure 

4.���� skynet
make 'macosx'

5.Ϊ������mac������
ȥ�� lua �� luac ��main ����

lua.c
#ifdef LUA_DEBUG
int mainlua (int argc, char **argv) {
#else
int main (int argc, char **argv) {
#endif

luac.c
#ifdef LUA_DEBUG
int mainluac(int argc, char* argv[])
#else
int main (int argc, char **argv)
#endif

6.xcode����
ֱ�Ӵ�skynet/skynet.xcodeproj �������