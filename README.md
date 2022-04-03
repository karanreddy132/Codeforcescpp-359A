# Codeforcescpp-359A
#include <bits/stdc++.h>
using namespace std;

int main() {
  int n,m,nums[50][50],flag(0);
  cin >> n >> m;
  for(int i=0;i<n;i++){
    for(int j=0;j<m;j++){
      cin >> nums[i][j];
      if(nums[i][j]==1 && (i==0 || i==n-1 || j==0 || j==m-1) && flag==0){
        cout << 2;
        flag = 1;
      }
    }
  }
  if(flag==0)
    cout << 4;
	return 0;
}
