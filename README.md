# ENCAPSULATION
#include<iostream>
using namespace std;
class flatform{
	private:
	string password;
	public:
		string founder;
		int no_users,no_programs;
		void setpass(string pass){
			password=pass;
		}
		string getpass(){
			return password;
		}
		flatform(string f,int u,int p)
		{
			founder=f;
			no_users=u;
			no_programs=p;
		}
		void founder_name()
		{
			cout<<founder<<" ";
		}
		void no_user()
		{
			cout<<no_users<<" ";
		}
};
int main()
{
	flatform codemind("Babji Neelam",1000,2213);
	codemind.founder_name();
	codemind.no_user();
	int po=codemind.no_programs;
	codemind.setpass("something");
	cout<<codemind.getpass();
	//cout<<codemind.password;
}
