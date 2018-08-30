#include <iostream>

using namespace std;

int main(){

int n;
bool runner = true;

cout << " ***********Rex Prime Number Checker***********\n" << endl;

while(runner){
    int c = 2;
    int checker = 1;
    cout << "Please enter a number or enter any other key to quit.."<< endl;
    cin >> n;
    if (n){
        for (c; c<=(n/2); c++){
            if ((n % c) == 0){
                checker = 0;
                break;
            }
        };
        if (checker == 1){
            cout << "Number is prime\n" << endl;
        }
        else{
            cout << "Number is not prime\n" << endl;
        }
    }
    else{
        cout << "You quit the program" << endl;
        runner = false;
    }
}
return 0;
};
