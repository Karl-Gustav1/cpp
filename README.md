# cpp
for C++ practice
1.const含义
常类型是指使用类型修饰符const说明的类型，常类型的变量或对象的值是不能被更新的。

2.const作用
可以定义常量
const int a=100;

防止修改，起保护作用，增加程序健壮性

void f(const int i){
    i++; // error!
}
可以节省空间，避免不必要的内存分配

const定义常量从汇编的角度来看，只是给出了对应的内存地址，而不是像#define一样给出的是立即数。
const定义的常量在程序运行过程中只有一份拷贝，而#define定义的常量在内存中有若干个拷贝。
