#include<bits/stdc++.h>
using namespace std;

using ll = long long int ;

class TC{

    public :
    void solve(){
        ll n , q ; cin >> n >> q ;
        vector<int> color(51,1e9) ;
        for(int i = 0 ; i < n; i++){
            int x ; cin >> x ;
            color[x] = min(color[x] , i + 1) ;
        }

        for(int i = 0 ; i < q ; i++){
            int query ; cin >> query ;
            int temp = color[query] ;
            cout << temp << " ";
            color[query] = 1 ;
            for(int j = 1 ; j < 51 ; j++){
                if(j == query) continue ;
                if(color[j] < temp){
                    color[j] ++ ;
                }
            }
        }
        cout << endl ;
    }
};

int main(){
    ios_base::sync_with_stdio(false);

    int testcases = 1;
    for(int i = 1 ; i <= testcases ; i ++){
        TC tc;
        tc.solve() ;
    }

    return 0 ;
}
