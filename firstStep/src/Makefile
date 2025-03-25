
# cross compiler 
CROSS_COMPILE=arm-linux-gnueabihf-

CFLAGS_DEBUG = -g -Wall

# 目标文件
all:hello1 hello  hello_c  clean

hello:hello.c
	gcc hello.c -o hello $(CFLAGS_DEBUG)
	@cp hello ../bin/.

hello_c:hello.c
	${CROSS_COMPILE}gcc  hello.c -o hello_c $(CFLAGS_DEBUG)
	@cp hello_c ../bin/.

clean:
	@rm -f hello hello1  hello_c

