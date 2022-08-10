# rokuban-casinoprogram]
#include <iostream>
#include <random>
#include <time.h>
#include <unistd.h>
#include <vector>
#include <algorithm>
using namespace std;
namespace {
 int x;
int y;
int Adice ;
int Bdice ;
int result ;
int answer ;
vector<int> dice;
}
int GetRandom(int min, int max);
int rollDice();
int main(void) {

cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　丁半　やってくかい？" << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
cout << "ハイ＝＞1　いいえ＝＞２\n" << endl;
  cin >> x;
  if(x == 1){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　   ダイスの数は？  " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" <<endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）\n"<< endl;
  cin >> y;
    }
  if(x == 2){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　     あばよ       " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
    sleep(3);
    exit(0);
  }
  
  int z;
    int i;
  int num;
    srand((unsigned int)time(NULL));
  do{
 dice.push_back( GetRandom(1, 6) );
  result += dice[num];
    //cout << dice[num] << endl;
     num += 1;
    }while(num< y);
  answer = result % 2;
  //cout << answer << endl;
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 はったはった      " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
  cout << "丁＝＞1　半＝＞0\n" << endl;
  cin >> z;
  if (z == 1){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 丁だな？結果は..." << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
  }
  if (z== 0){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 半だな？結果は..." << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
  }
  sleep(3);
  for(num = 0; num < y;num += 1){
        int face = dice[num];
        switch(face){
        case 1:
      cout << "+---+" << endl; 
      cout << "|   |" << endl;
      cout << "| O |" << endl;
      cout << "|   |" << endl;
      cout << "+---+" << endl;
            break;
        case 2:
      cout << "+---+" << endl; 
      cout << "|  O|" << endl;
      cout << "|   |" << endl;
      cout << "|O  |" << endl;
      cout << "+---+" << endl;
            break;
        case 3:
      cout << "+---+" << endl; 
      cout << "|  O|" << endl;
      cout << "| O |" << endl;
      cout << "|O  |" << endl;
      cout << "+---+" << endl;
            break;
        case 4:
      cout << "+---+" << endl; 
      cout << "|O O|" << endl;
      cout << "|   |" << endl;
      cout << "|O O|" << endl;
      cout << "+---+" << endl;
            break;
        case 5:
      cout << "+---+" << endl; 
      cout << "|O O|" << endl;
      cout << "| O |" << endl;
      cout << "|O O|" << endl;
      cout << "+---+" << endl;
            break;
        case 6:
      cout << "+---+" << endl; 
      cout << "|O O|" << endl;
      cout << "|O O|" << endl;
      cout << "|O O|" << endl;
      cout << "+---+" << endl;
            break;
	      return face;
          }}
  if (0 == answer){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 合計は"<< result <<"  半だ"<< endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
    if(0 == z){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 正解だ           " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
      }
  else{
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 不正解だ           " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
    } 
    }
  
  if(1 == answer){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 合計は"<< result <<"  丁だ"<< endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;  
    if(1 == z){
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 正解だ           " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl; 
      }
  else{
cout <<"  ∧＿∧  　 ／￣￣￣￣￣￣￣￣￣￣"<< endl;
cout <<"（ ´∀｀ ）＜　 不正解だ           " << endl;
cout <<"（      ）　＼＿＿＿＿＿＿＿＿＿＿" << endl; 
cout <<" ｜ ｜  |" << endl;
cout <<"（_＿）＿）"<< endl;
    }
    }
      return 0;
}

int GetRandom(int min, int max)//乱数を計算するところ
{
return min + (int)(rand() * (max - min + 1.0) / (1.0 + RAND_MAX));
}
