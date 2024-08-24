#include<iostream>
#include<fstream>
#include<string.h>
using namespace std;

void login();
void registration();
void forget();

int main()
{
	cout<<"\t___________\n" ;
	cout<<"\t||welcome||\n" ;
	cout<<"\t___________\n" ;
	cout<<"login and Registration\n" ;
	cout<<"\n" ;
	cout<<"\n" ;
	cout<<"\tpress 1 login           :: \n" ;
	cout<<"\tpress 2 registeration   :: \n" ;
	cout<<"\tpress 3 forget password :: \n" ;
	cout<<"\tpress 4 to exit         :: \n\n" ;
	cout<<"\n\tPlease enter your choice::" ;
int c;cin>>c;
cout<<endl;

switch(c)
{
	case 1:
		login();
		break;
	case 2:
		registration();
		break;
	case 3:
		forget();
		break;
	case 4:
		cout<<"thankyou\n";
		break;
	default:
		system("cls");
		cout<<"\tplease select from the op"<<endl;
		main();
}}
void login()
{
	int count;
	string userId,password,id,pass;
	system("cls");
	cout<<"\t please enter username and password\n"<<endl;
	cout<< "user name\n";
	cin>>userId;
	cout<< "password\n";
	cin>>password;
	
	ifstream input("record.txt");
	
	while ( input>>id>>pass)
	{
		if(id==userId&& pass==password)
		{
			count=1;
			system("cls");
		}
	}
	input.close();
	
	if(count==1)
	{
		cout<<userId<<":: your login sucessful\n\n\n";
		cout<<"Going back to main menu\n\n";
		main();
	}
	else{
		cout<<"\n login error\nplease check again your username and password\n";
		main();
	}
	}
	void registration()
	{
		string ruserId,rpassword,rid,rpass;
		system("cls");
		cout<<"\t enter your username:";
		cin>>ruserId;
		cout<<"enter your password:";
		cin>>rpassword;
		
		ofstream f1("record.txt",ios::app);
		f1<<ruserId<<' '<<rpassword<<endl;
		system("cls");
		cout<<"\nRegistration is successfull\n";
		main();
		
	}
	
	void forget(){
	
	system("cls");
	cout<<endl;
	cout<<"\t\n no worry\n\n";
	cout<<"\npress 1 to search by username\n"<<endl;
	cout<<"press 2 to back to menu\n"<<endl;
	cout<<"enter option ::";
	int option;
cin>>option;
switch(option)
{
	case 1:
	{
		int count=0;
		string suserId,sId,spass;
		cout<<"\n\tenter user name:";
		cin>>suserId;
		
		ifstream f2("record.txt");
		while(f2>>sId>>spass)
		{
			if(sId==suserId)
			{
				count=1;
			}
		}
		f2.close();
		if(count==1)
		{
			cout<<"\n\n account found!\n";
			cout<<"\n\n your password is:"<<spass<<endl;
			main();
		}
		else{
			cout<<"\nsorry! account not found:\n";
			main();
		}
		break;
	}
	case 2 :
		{
			main();
		}
		default:
			cout<<"wrong choice! try again"<<endl;
			main;
		}}
