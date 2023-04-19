# reversestring

class Solution {
public:
    void f(int i, vector<char>&s){
     if(i>=s.size()/2)//mid
     return ;
     swap(s[i], s[s.size()-i-1]);//swaping
     f(i+1,s );
    }
    void reverseString(vector<char>& s) {
      f(0, s);//calling func

    }
};
