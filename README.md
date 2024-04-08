# C-project

#include<iostream>

using namespace std;

int main(){
char startValue;
char choiceAgain;
double onlineShopping(void);
startLevel:
cout<<"Please press s to start Shopping"<<endl;
start:
cin>>startValue;
if(startValue=='s' || startValue=='S'){
double totalAmount=onlineShopping();
cout<<"Total BillAmount is "<<totalAmount<<endl;
shopAgain:
cout<<"Do you want shopping again, y or n"<<endl;
cin>>choiceAgain;
if(choiceAgain=='y' || choiceAgain=='Y'){
goto startLevel;
}
else if(choiceAgain=='n' || choiceAgain=='N'){
cout<<"Thanks for shopping"<<endl;
}
else {
cout<<"You have entered wrong option, please type again"<<endl;
goto shopAgain;
}
}
else{
cout<<"You have entered wrong option, please s"<<endl;
goto start;
}
}

double onlineShopping(){
    char choice;
    char item;
    int quantity;
    double billAmount=0;
    itemLevel:
    cout<<"****************Welcome to Online Shopping***************"<<endl;
    cout<<"----------Please follow the instructions------------"<<endl;
    cout<<"(1) Please enter m to order mobile phones"<<endl;
    cout<<"(2) Please enter l to order laptops"<<endl;
    cout<<"(3) Please enter d to order desktops"<<endl;
    cout<<"(4) Please enter s to order Speaker"<<endl;
    cout<<"(5) Please enter h to order Headphone"<<endl;
    cin>>choice;

//**********************************Mobile*******************************//
if(choice=='m' || choice=='M'){
mobileLevel:
cout<<"Mobile details"<<endl;
cout<<"(1) Apple   =>  Price  : 40000"<<endl;
cout<<"(2) Vivo    =>  Price  : 25000"<<endl;
cout<<"(3) Oppo    =>  Price  : 20000"<<endl;
cout<<"(4) Redmi   =>  Price  : 18000"<<endl;
cout<<"(5) Realme  =>  Price  : 170000"<<endl;
cout<<"(6) Samsung =>  Price  : 25000"<<endl;
cout<<"Please enter your  number of choice"<<endl;
cin>>item;
if(item=='1'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*40000;
}
else if(item=='2')  {
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*25000;
}

else if(item=='3'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*20000;
}

else if(item=='4') 
{
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*18000;
}
else if(item=='5'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*17000;
}
else if(item=='6'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*25000;
}
else{
cout<<"You have entered wrong option, please type again"<<endl;
goto mobileLevel;
}
}

//**********************************Desktop*******************************//
else if(choice=='d' || choice=='D'){
desktopLevel:
cout<<"Desktop details"<<endl;
cout<<"(1) L.G   =>  Price  : 25000"<<endl;
cout<<"(2) apple    =>  Price  : 80000"<<endl;
cout<<"(3) dell    =>  Price  : 30000"<<endl;
cout<<"(4) H.P   =>  Price  : 20000"<<endl;
cout<<"(5) soni  =>  Price  : 17000"<<endl;
cout<<"(6) zebronics =>  Price  : 25000"<<endl;
cout<<"Please enter your number of choice"<<endl;
cin>>item;
if(item=='1')
{
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*25000;

}
else if(item=='2'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*80000;
}

else if(item=='3'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
illAmount=billAmount+quantity*30000;
}

else if(item=='4'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*20000;
}
else if(item=='5'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*17000;
}
else if(item=='6'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*25000;
}
else{
cout<<"You have entered wrong option, please type again"<<endl;
 goto desktopLevel;
}
}


//**********************************laptops*******************************//

else if(choice=='l' || choice=='L'){
laptopLevel:
cout<<"Laptop details"<<endl;
cout<<"(1) Apple   =>  Price  : 90000"<<endl;
cout<<"(2) dell    =>  Price  : 25000 "<<endl;
cout<<"(3) H.P    =>  Price  : 28000"<<endl;
cout<<"(4) lenovo   =>  Price  : 30000"<<endl;
cout<<"(5) asus  =>  Price  :   80000"<<endl;
cout<<"(6) acer =>  Price  :   23000"<<endl;
cout<<"Please enter your number of choice"<<endl;
cin>>item;
if(item=='1'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*90000;

}
else if(item=='2'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*25000;
}

else if(item=='3'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*28000;
            
}

else if(item=='4')  
{
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*30000;
}

else if(item=='5'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*80000;
}

else if(item=='6'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*23000;
}
else
{
cout<<"You have entered wrong option, please type again"<<endl;
goto laptopLevel;
}
}


//**********************************Speaker*******************************//

else if(choice=='s' || choice=='S'){
speakerLevel:
cout<<"Speaker details"<<endl;
cout<<"(1) J.B.L   =>  Price  : 5000"<<endl;
cout<<"(2) boat    =>  Price  : 3000"<<endl;
cout<<"(3) bose    =>  Price  : 7000"<<endl;
cout<<"(4) apple   =>  Price  : 25000"<<endl;
cout<<"(5) sonose  =>  Price  : 100000"<<endl;
cout<<"(6) zebronics =>  Price  : 2000"<<endl;
cout<<"Please enter your number of choice"<<endl;
cin>>item;
if(item=='1'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*5000;
}

else if(item=='2')   {
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*3000;
}

else if(item=='3') 

{
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*7000;
}

else if(item=='4'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*25000;
}

else if(item=='5'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*100000;
}
else if(item=='6')
        
{
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*2000;

}
else
{
cout<<"You have entered wrong option, please type again"<<endl;
goto speakerLevel;
}
}


//**********************************Headphone*******************************//

else if(choice=='h' || choice=='H'){
headphoneLevel:
cout<<"Headphone details"<<endl;
cout<<"(1) audio technical   =>  Price  : 8000"<<endl;
cout<<"(2) beates   =>  Price  : 2000"<<endl;
cout<<"(3) jebra    =>  Price  : 4000"<<endl;
cout<<"(4) sony   =>  Price  : 7000"<<endl;
cout<<"(5) apple  =>  Price  : 50000"<<endl;
cout<<"(6) bose =>  Price  : 25000"<<endl;
cout<<"Please enter your number of choice"<<endl;
cin>>item;
if(item=='1'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*8000;

}
else if(item=='2'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*2000;
}

else if(item=='3'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*4000;
}

else if(item=='4'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*7000;
}
else if(item=='5'){
cout<<"Enter quantity"<<endl;
cin>>quantity;
billAmount=billAmount+quantity*50000;
}
else if(item=='6'){
            cout<<"Enter quantity"<<endl;
            cin>>quantity;
            billAmount=billAmount+quantity*25000;
}
else{
            cout<<"You have entered wrong option, please type again"<<endl;
            goto headphoneLevel;
}
}
else{
            cout<<"You have entered wrong option, please type again"<<endl;
            goto itemLevel;
}
return billAmount;
}

 

