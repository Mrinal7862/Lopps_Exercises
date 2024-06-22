<h1>Loops Pattern</h1>

### First: Simple Triangle Pattern

    *
    **
    ***
    ****
    *****

        
```c++
#include <iostream>

using namespace std;

int main(){

    int n;
    
    cin>>n;

    for(int i=1; i<=n; i++){

        for(int j=1; j<=i; j++){

            cout<<"*";
        }

    cout<<endl;

    }
    return 0;
}
```


### Second : Equalateral Triangle
```
    *
   ***
  *****
 *******
*********
```

```c++
int main(){
    
    int n;

    cin>>n;

    for(int i=1; i<=n; i++){

        for(int j=1; j <= n; j++){
            cout<<' ';

        }

        for(int j=1; j<= 2* i-1; j++){
            cout<<"*";
        }

        cout<<endl;
    }
}
```
### Third : Reverse Triangle
```
    *
   **
  ***
 ****
***** 
```

```c++

for(int i=1; i<=n; i++){

    for(int j=1; j<=n; j++){

        if(j<=n-i){
            cout<<" ";
        }

        else{
            cout<<"*";
        }
    }
    cout<<endl;
}
```

### Fourth : Floyd's Triangle
```
1
2 3
4 5 6
7 8 9 10
11 12 13 14 15
```
```c++
int n;

cin>>n;

int count = 1

for(int i = 1; i<= n; i++){

    for(int j=1; j<= n; j++){

        cout<<count;
        count++

    }
cout<<endl;
}
```

### Fifth :  Butterfly Triangle 

``` 
*        *
**      **
***    ***
****  ****
**********
**********
****  ****
***    ***
**      **
*        *
```
```c++
   int n;

    cin>>n;

    for(int i=1; i<=n; i++){
        for(int j = 1; j<=i; j++){
            cout<<"*";
        }
        int space = 2*n - 2*i;

        for(int j = 1; j<=space; j++){
            cout<<" ";
        }

        for(int j = 1; j<=i; j++){
            cout<<"*";
        }
        cout<<endl;
    }

    for(int i=n; i>=1; i--){
        for(int j=1; j<=i; j++){
            cout<<"*";
        }

        int space = 2*n - 2*i;
        for(int j = 1; j<= space; j++){
            cout<<" ";
        }

        for(int j = 1; j<= i; j++){
            cout<<"*";
        }
        cout<<endl;
    }

```

### Sixth : Number Triangle

```c++
int main(){

    int n;
    cin>>n;

    for(int i=1; i<=n; i++){

        for(int j=1; j<=i; j++){
            cout<<i;
        }

    cout<<endl;
    }
```