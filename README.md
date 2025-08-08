福建兄妹系列全集视频

//C++98 考虑把父类的构造函数私有化即可
//这样的话，这个类继承就几乎没有意义了
//间接使得父类不能被继承
class A
{
private:
	A()
	{}
protected:
//这里也可以私有化，这样连成员变量也是不可见的
	int _a;
	int _b;
};
 
class B :public A
{
 
};
 
int main()
{
	//B bb;//此时不管调用默认的还是显式书写的，都定义不出对象
 
	return 0;
}
