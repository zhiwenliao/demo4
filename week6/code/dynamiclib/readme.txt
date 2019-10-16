生成动态库指令：gcc -shared -fPIC -o libdylib.so aopend.c base.c
在当前目录下链接当前动态库：gcc ldtextlocal.c -o ldtextlocal ./libdylib.so
