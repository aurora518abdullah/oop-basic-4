#include<iostream>
using namespace std;
class bankaccount
{
  private:
    string accountholder;
    int balance;
    
    
  public:
     bankaccount(string s,int n)
    {
        accountholder=s;
        balance=n;
    }
    
    
    int getbalance()
    {
        return balance;
    }
    
     void deposit(int amount) 
     {
        balance += amount;
    }
};
int main()
{
    bankaccount a("Rahim",1000);
    a.deposit(6609);
    cout<<"balance: "<<a.getbalance();
}
