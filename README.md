# C-project

#include<iostream>
using namespace std;

int main(){
    char startevalue;
    char choiceagain;
    float onlineshopping(void);
    startlevel:
    cout<<"please press 's' to start shoping"<<endl;
    start:
    cin>>startevalue;
    if(startevalue== 's' || startevalue== 'S'){
        float totalamount=onlineshopping();
        shopeagain:
        cout<<"total billamount<<"totalamount<<endl;
        cout<<"do you want to shopping again y or n"<<endl;
        cin>>choiceagain;
        if(choiceagain== 'y'  || choiceagain= 'Y'){
            goto startlevel;

  }
        else if(choiceagain== 'n'  || choiceagain= 'N'){
            cout<<"thanks for shopping"<<endl;
        }
        else{
            cout<<"you have enter wronge option, please type again"<<endl;
            goto shopeagain;

  }
    }
    else 
    {
        cout<<"you have enter wronge option, please s"<<endl;
        goto start;
    }
    
}
float onlineshopping(){
    char choise;
    char item;
    int quantity;
    float billamount=0;
    cout<<"*************welcome to online shopping******************"<<endl;
    cout<<"-------------please follow the instruction--------------"<<endl;
    cout<<"(1) please enter m to order mobile phone"<<endl;
    cout<<"(2) please enter l to order mobile laptop"<<endl;
    cout<<"(3) please enter d to order mobile destops"<<endl;
    cout<<"(4) please enter s to order mobile speaker"<<endl;
    cout<<"(5) please enter h to order mobile headphone"<<endl;
    cin>>choise;
// ****************************mobile*****************************
if(choise=='m'  || choise=='M'){
    mobilelevle:
    cout<<"mobile details"<<endl;
    cout<<"(1) Apple   =>   prise :  40000"<<endl;
    cout<<"(2) vivo   =>   prise :  25000"<<endl;
    cout<<"(3) oppo   =>   prise :  20000"<<endl;
    cout<<"(4) redmi   =>   prise :  18000"<<endl;
    cout<<"(5) realmi   =>   prise :  17000"<<endl;
    cout<<"(6) samsung   =>   prise :  15000"<<endl;
    cout<<"please enter your choice"<<endl;
    cin>>item;
    if(item =='1'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*40000;

}
    else if(item =='2'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*25000;

  } else if(item =='3'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*20000;
 } else if(item =='4'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*18000;
        }
        else if(item =='5'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*17000;
        }
        else if(item =='6'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*15000;
        }
        else{ 
            cout<<"you have enter wronge option, please type again"<<endl;
            goto mobilelevle;

        }
        // ****************************desktop*****************************
if(choise=='d'  || choise=='D'){
    destoplevle:
    cout<<"desktop details"<<endl;
    cout<<"(1) L.G   =>   prise :  12000"<<endl;
    cout<<"(2) soni   =>   prise :  25000"<<endl;
    cout<<"(3) zibronics   =>   prise :  21000"<<endl;
    cout<<"(4) Apple    =>   prise :  80000"<<endl;
    cout<<"(5) dell   =>   prise :  17000"<<endl;
    cout<<"(6) H.P   =>   prise :  15000"<<endl;
    cout<<"please enter your choice"<<endl;
    cin>>item;
    if(item =='1'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*12000;

  }
    else if(item =='2'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*25000;

  } else if(item =='3'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*21000;
 } else if(item =='4'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*80000;
        }
        else if(item =='5'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*17000;
        }
        else if(item =='6'){
        cout<<"enter quantity"<<endl;
        cin>>quantity;
        billamount=billamount+quantity*15000;
        }
        else{ 
            cout<<"you have enter wronge option, please type again"<<endl;
            goto destopevle;
            }
   
  return billamount;
}
