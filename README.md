# leetcode_problem-shuffel-string-
# use of map
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


#include <bits/stdc++.h>
using namespace std;

int main()
{
    
    vector<int> indices = {4,5,6,7,0,2,1,3};
    string s = "codeleet";
    
    string str;
    
        int n = indices.size();
        
        map<int , char> m;
        for(int i=0; i<n; i++){
            m[indices[i]] = s[i];
        }
        
        for(auto i : m){
            str.push_back(i.second);
        }
        
         for(auto i : str){
            cout<<i;
        }cout<<endl;

    return 0;
}
