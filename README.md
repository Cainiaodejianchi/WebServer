# WebServer
使用c++实现一个web服务器

分支 ：V01 
用途 ：本地代码修改

g++ 与 gcc 的区别 ： 

1. 后缀为.c的，gcc把它当做C程序，而g++当做是C++程序；后缀是.cpp的，都会认为是c++程序。
2. gcc命令不能自动和c++程序使用的库链接，所以通常用g++来完成链接
3. 用extern “C” ,告知编译器以C的方式为symbol命名编译
#ifdef __cplusplus
extern "C" {
#endif

#ifdef __cplusplus
}
#endif
4. 不同C++标准中__cplusplus值是不同的
5. 如果后缀为.c ，并且采用gcc 编译器，则该宏__cplusplus就是未定义的，否则就是已定义。
