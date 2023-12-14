#include <iostream>
#include <string>


class GenericThing
{
private:
    int privateData = 123456789;
    void print()
    {
        std::cout << data1 << " " << data2 << std::endl;
    }

public:
    int data1;
    int data2;

    int getPrivateData()
    {
        return privateData;
    }
    int getData1()
    {
        return data1;
    }
    int getData2()
    {
        return data2;
    }
    void setData1(int input)
    {
        data1 = input;
    }
    void setData2(int input)
    {
        data2 = input;
    }
    void doSomething()
    {
        print();
    }
};

class DerivedThing1 : public GenericThing
{
public:
    int doSomething()
    {
        int sum = getData1() + getData2();
        return sum;
    }
};

class DerivedThing2 : public GenericThing
{
public:
    int doSomething()
    {
        int diff = getData1() - getData2();
        return diff;
    }
};


int main()
{
    GenericThing og;
    DerivedThing1 obj1;
    DerivedThing2 obj2;

    og.setData1(1);
    og.setData2(2);
    obj1.setData1(1);
    obj1.setData2(2);
    obj2.setData1(1);
    obj2.setData2(2);

    std::cout << "this is printed from a function hidden through abstraction: ";
    og.doSomething();
    std::cout << "this is encapsulated data: " << og.getPrivateData() << "\n" <<
        "the following are calculated in a method with multiple forms (polymorphism)" << "\n" <<
        "derived class 1: " << obj1.doSomething() << "\n" <<
        "derived class 2: " << obj2.doSomething() << "\n" << std::endl;
        
    return 0;

}
