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
   **std::cout <<"Hello World!"<<std::endl;** fakat bu bizi biraz yoracağından en başa **using namespace std;** yazmak bizim açımızdan çok daha rahat olacaktır.
