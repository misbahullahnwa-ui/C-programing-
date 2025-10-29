//# C-programing-
//this is my c++ programing for my practice only 
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string name;
    float balance, amount;
    int choice;
    cout<<"Enter your name \n";
    cin>>name;
    cout<<"Enter your current amount balance"<<endl;
    cin>>balance;
    cout << "\n ----Menu of ATM ---"<<endl;
    cout<<"1.n Deposit Money\n";
    cout<<"2.Withdraw Money\n";
    cout<<"3. Check Balance\n";
    cout<<"Enter your choice (1 , 2, or 3): ";
    cin>>choice;

    if(choice==1)
    {
        cout<<"\nEnetr amount to deposite ";
        cin>>amount;
        balance=balance+amount;
        cout<<"Depoiste Successfull ! \n";
        cout <<" Your balace is : "<<balance<<"\n";
        cin>>balance;
        
    }
    else if(choice==2)
    {
        cout <<" \n Enter amount to withdraw ";
        cin>>amount;
        if(amount > balance )
        {
            cout<<" Insufficient balance!\n";
            cout<<"Remaining balance:"<<balance<<"\n";
            
            cin>>balance;

        }

    }
    else if(choice==3)
    {
        cout<<"\nYour current balnce is: "<<balance<<"\n";
        cin>>balance;

    }
    else
    {
        cout<<"\nInvalid choice! please select 1, 2 , or 3, \n";

    }
    cout<<"\nThank you for using our ATM service";
    return 0;
    
}
