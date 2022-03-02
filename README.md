# c++ code

----

## c++ ile Merhaba dünya yazdırılması

ilk olarak c++ dilinin kemik yapısını gösterelim.

#include <iostream>
using namespace std;
int main() 
{
  cout <<"Hello World!"<< endl;
  return 0 ;
}  

Kodumuzu kemik tarafı böyle eğer bunları açıklayacak olursak **iostream** bizim buradaki temel işlemleri alan bir kütüpahnemiz.
**using namespace std;** ise bize kolaylık sağlayın bir kodumuz yani yazmak zorunda olmadığımız bir kod. Fakat eğer yazmasak konsoldan çıktı almak için yazacağımız kod için şöyle yazmamız gerek  :
   **std::cout <<"Hello World!"<<std::endl;** fakat bu bizi biraz yoracağından en başa **using namespace std;** yazmak bizim açımızdan çok daha rahat olacaktır. Ek olarak bir yazdırma işlemi yaparken en sona **endl;** yazmıştık bunun anlamı ise bir sonraki satıra geçtir.
  
  ----
  
  ## c++ dilinde yorum yazılması :
  
 Yorum satırları : Eğer bir kod içersinde çalışmayacak  tek bir satıra yorum eklemek isterseniz  **//** işareti koymanız yeterli olur . Eğere çok satırlı bir yorum yapmak isterseniz :
  /*
  
  */
yapabilirsiniz bu size iki işaret arasına istediğiniz yorumu yazmanıza yardımcı olacaktır.

----
  

## İkilik taban işlemleri :
  
  XOR(exclusive or) (^):
  00 --> 0
  10 --> 1
  10 --> 1
  00 --> 0
  
  and(&):
  00 --> 0
  10 --> 0
  01 --> 0
  11 --> 1
  
  or (|) :
  00 --> 0
  10 --> 1
  01 --> 1
  11 --> 1
  
----

  
## Temel Giriş ve Çıkış İşlemleri :

  Daha önceden gördüğümüz bir yazıyı bastırma komutunun **cout<<"yazılacak_yer"<<** endl; olduğunu biliyoruz. Fakat biz kullanıcıdan bir sayı almak istersek napıcaz. 
  Hemen bir örnek yapalım
  
  #include <iostream>

using namespace std;

int main()
{
float a;
float b;
cout<<"lütfen birinci sayiyi giriniz :"<< endl;
cin >>a;
cout<<"lütfen ikinci sayiyi giriniz :"<< endl;
cin >>b;                                                                                       bu örnekte kullandığım cin fonksiyonu bize kullanıcıdan bir değer almamızı
cout<<"girdiginiz 1. sayi :"<<a<< endl;
cout<<"girdiginiz 2. sayi :"<<b<< endl;                                                        sağlayacaktır.                                                 
cout<<a<<" ile "<<b <<" sayisinin toplami :  "<<a+b<<endl;
cout<<a<<" ile "<<b <<" sayisinin farkı :  "<<a-b<<endl;
cout<<a<<" ile "<<b <<" sayisinin bolumu :  "<<a/b<<endl;
cout<<a<<" ile "<<b <<" sayisinin carpimi :  "<<a*b<<endl;
return 0;
}
  
  
----
  
## İf - Else yapıları :
  
  İf else yapsını  kısaca bir örnekle açıklayıp geçelim
  
  
  #include <iostream>

using namespace std;

int main()
{
float vize1,vize2,vize3;
float ortalama;
cout<<"1.vize notunuzu giriniz :"<<endl;
cin >>vize1;
cout<<"2.vize notunuzu giriniz :"<<endl;
cin >>vize2;
cout<<"final notunuzu giriniz :"<<endl;
cin >>vize3;
ortalama=(vize1+vize2+vize3)/3;

if(ortalama<50)
{
    cout<<"harf notunuz : 'F' "<<endl;
}
else if(ortalama>=50 && ortalama <70)
{
    cout<<"harf notunuz : 'C' "<<endl;
}
else if(ortalama >=70 && ortalama <90 )
{
     cout<<"harf notunuz : 'B' "<<endl;
}
else
{
     cout<<"harf notunuz : 'A' "<<endl;
}

return 0;
}

  
  
  
  
  
  
  
  
  
  
  
