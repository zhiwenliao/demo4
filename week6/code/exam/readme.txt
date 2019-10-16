将某一个目录下的文件拷贝到当前目录：cp ../staticlib/localtest.c ./remotetest.c
先在测试目录下验证gcc remotetest.c -o remotetest1出错是因为没有链接到库文件
所以要链接：gcc remotetest.c -o remotetest1 -L../staticlib/ -lstatic -I../staticlib/
