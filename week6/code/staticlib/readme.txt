对文件进行编译：gcc -c base.c aoprand.c
生成动态库(库名为：staticlib.a)：ar -rc staticlib.a aoprand.o base.o
动态库的命令规则：mv staticlib.a libstatic.a
gcc -c test.c将生成test.o的目标文件
gcc -o app test.c将生成可执行程序app
拷贝home目录下的文件到当前目录：cp ../statilib/localtest.c ./remotetest.c

