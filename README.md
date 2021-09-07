# Assignment2_problem1
 Print the sum, difference, and product of two complex numbers by creating a class named 'Complex' with separate methods for each operation whose real and imaginary parts are entered by user.
 
#include<iostream>
using namespace std;
class Complex{
    int real, imaginary ;
    public:
    void setData(){
        cout<<"Enter the real and imaginary part of numbers"<<endl;
        cin>>real;
        cin>>imaginary;
        

        }
    
    void sum (Complex C1, Complex C2){
        real = C1.real +C2.real;
        imaginary= C1.imaginary+C2.imaginary;
        cout<<" The sum is "<<real<<"+"<< imaginary<<"i"<<endl;

    }
    void diffrence (Complex C1, Complex C2) {
        real = C1.real -C2.real;
        imaginary= C1.imaginary-C2.imaginary;
        cout<<" The diffrence is "<<real<<"-"<< imaginary<<"i"<<endl;

    }
    void product  (Complex C1, Complex C2)
    {
        real=((C1.real)*(C2.real))-((C1.imaginary)*(C2.imaginary));
        imaginary=((C1.real)*(C2.imaginary))+((C2.real)*(C1.imaginary));
        cout<<"the product is"<<real<<"+"<<imaginary<<"i"<<endl;
    }
    };

int main(){
    Complex C1,C2,C3,C4,C5;
    cout<<"This is a First number "<<endl;
    C1.setData();
    cout<<"This is a Second number "<<endl;
    C2.setData();
    C3.sum(C1,C2);
    C4.diffrence(C1,C2);
    C5.product(C1,C2);
    return 0;
}
