CC = gcc
libs_for_gnu = -lgnu				#使用gnu函数库
normal_libs = 
objects = main.o list.o my_lib.o	# 所有的目标文件
app : $(objects) 
ifeq ($(CC), gcc) 				# 使用gnu的函数库
	$(CC) -o app $(objects) $(libs_for_gcc)
else 
	$(CC) -o app $(objects) $(normal_libs) 
endif 
main.o : main.c 					
	$(CC) -c main.c					# 生成main.o
list.o : list.c
	$(CC) -c list.c					# 生成list.o
my_lib.o : my_lib.c
	$(CC) -c my_lib.c				# 生成my_lib.o
