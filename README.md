# rokuban-casinoprogram]
#include <iostream>
#include <random>
#include <time.h>
using namespace std;
namespace {
int Adice ;
int Bdice ;
int result ;
int answer ;
}
int GetRandom(int min, int max);
int main(void) {
  int z = 0;
    int i;

    srand((unsigned int)time(NULL));

        Adice = GetRandom(1, 6);
        Bdice = GetRandom(1, 6);
  
  answer = result % 2;
  cout << answer << endl;
  cout << "はったはった" << endl;
  cout << "丁＝＞1　半＝＞0\n" << endl;
  cin >> z;
  cout << Adice << endl;
  cout << Bdice << endl;
  if (0== answer){
    cout << result << "    半だ" << endl;
    }if(0 == z){
      cout <<  "正解だ" << endl;
      }else{
      cout << "不正解だ" << endl;
      } 
  if(1 == answer){
    cout << result << "    丁だ" << endl;
    }if(1 == z){
      cout <<  "正解だ" << endl;
      }else{
      cout << "不正解だ" << endl;
      }
  

      return 0;
}
int GetRandom(int min, int max)
{
    return min + (int)(rand() * (max - min + 1.0) / (1.0 + RAND_MAX));
}
void gambl(){
    int x;
  int y;
cout << "丁半　やってくかい？ " << endl;
cout << "ハイ＝＞1　いいえ＝＞２\n" << endl;
  cin >> x;
  switch (x){
    case 1:
    case 2:
    exit(0);
  }
}
