# vectors
#include<iostream>
#include<vector>
using namespace std;
int main()
{
//format:vector<datatype> nameofvector
//myvector.push_back(value)-->adds an element to thr END of vector(resizesit)
//myvector.at(index)-->return element at specified index number
//myvector.size()-->returns an unsigned int equal to number of elements
//myvector.begin()-->reads vector from first element(index 0)
//myvector.insert(myvector.begin()+integer,newvalue)
//myvector.erase(myvector.begin()+integer)-->removes element

vector<int> myvector;

myvector.push_back(3);
myvector.push_back(7);
myvector.push_back(6);
myvector.push_back(12);
myvector.push_back(26);
cout<<"vector: ";
for(unsigned int i=0;i<myvector.size();i++)
{
cout<<myvector[i]<<" ";
}
myvector.insert(myvector.begin() + 3,5);
cout<<endl<<"vector: ";
for(unsigned int i=0;i<myvector.size();i++)
{
cout<<myvector[i]<<" ";
}
myvector.erase(myvector.begin() + 4);
cout<<endl<<"vector: ";
for(unsigned int i=0;i<myvector.size();i++)
{
cout<<myvector[i]<<" ";
}
if(myvector.empty()){
cout<<endl<<"is empty!";
}
else{
cout<<endl<<"is not empty";
}
cout<<endl;
return 0;
}
