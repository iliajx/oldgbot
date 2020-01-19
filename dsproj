#include <iostream>
#include <string>
#include <vector>
#include <conio.h>
#include <fstream>
#include<windows.h>
#include <sstream>
using namespace std;
vector <string> words;

void fileOk(){
    fstream file("db.txt");
    if(file){
    string t;
    getline(file,t);
    string temp;
    istringstream text(t);
    while(getline(text,temp,',')){
        string tVec;
        string t2;
      //  cout << temp << endl;
        if(temp[0] < '0' && temp[0] > '9'){
            int i;
            cout << "Im here" << endl;
            for( i = 1;temp[i] > '0' && temp[i] <= '9';i++);//{
           //     if(temp[i] != ' ')break;
          //  }
        for(int j = i ; j < temp.size();j++){
            t2 += temp[j];
        }
        temp = t2;
        }

        cout << temp << ' ' << temp.size() << endl;
        if(temp[1] >= '1' && temp[1] <= '9')
        {
            for(int i= 2 ; i < temp.size() ; i++)
                tVec += temp[i];

            words.push_back(tVec);
        }else{
        for(int i = 1 ; i < temp.size() ; i++)
                tVec += temp[i];

            words.push_back(tVec);
        }
        cout << tVec << endl;
    }

}else{
cout << "ERROR TO OPEN FILE" << endl;}

}
void list(string x){



}


int main()
{
   SetConsoleOutputCP(65001);


    fileOk();
    string x;
    char t;

   /* for(int i = 0 ; i < words.size();i++){
        cout << words[i] << endl;
    }
*/
   /* while(t = getche()){

       x += t;

    }
*/


    return 0;
}
