## level3 solution
### 思路：
- 通过gdb调试获取出存储char* sval的寄存器
- 用汇编指令修改该寄存器的所指的内存单元的值，让其值与cookie相等（注意使用小端存储，记得添加结束符）
- 把返回touch3地址压栈中，最后返回即可