# AIM 
To create array in c++ and doing basic operations on it.

# Software Used
VS Code

# Problem Statement

1.) Write a c++ code to make an array.

2.) Write a c++ code to make an array with elements in reverse order in which user entered.

3.) Write a c++ code to make do sum and average of array elements.

4.) Write a c++ code to find maximum and minimum element of an array.

5.) Write a c++ code to search the position of element, number of time it is occuring in an array.
 
 6.) Write a c++ program to take input from user. 

 7.) Write a c++ program to concatenate the string on c++. 

 8.)  Write a c++ program to reverse string. 

 9.)  Write a c++ program to check a palindrome.


# Theory
In C++, an array is a data structure that is used to store multiple values of similar data types in a contiguous memory location.

 C++ strings are sequences of characters stored in a char array. Strings are used to store words and text. They are also used to store data, such as numbers and other types of information. Strings in C++ can be defined either using the std::string class or the C-style character arrays.

# Program Codes

```javascript
//Array
#include<iostream>
using namespace std;
int main()
{
    int n, i, j;
    cout << "Enter number of elements";
    cin >> n;
    int a[n];
    cout << " Enter array elements";
    for ( int i =0; i <n ; i++ )
    { cin >> a[i];
     
    }
       for (int i: a)
     {
        cout << " "<< i ;
     } 
    return 0;
}

//Reverse array
#include<iostream>
using namespace std;
int main()
{
    int n, i, j;
    cout << "Enter number of elements";
    cin >> n;
    int a[n];
    cout << " Enter array elements";
    for ( int i =0; i <n ; i++ )
    { cin >> a[i];
     
    }
       for (j = n-1 ; j>=0; j--)
     {
        cout << " "<< a[j];
     } 
    return 0;
}

//Sum & average of array elements
#include<iostream>
using namespace std;
int main()
{
     int n, i, j;
     float avg, s = 0;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}

for (j= 0 ; j<n; j++)
{
    s = a[j]+s;
}
avg = s/n;
cout << "The sum of elements of the given array is: "<<s<<endl;
cout << "The average of the given array is: "<< avg<<endl;

return 0;
}

//Maximum and minimum
#include<iostream>
using namespace std;
int main()
{
     int n, i, j, max, min;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}
max = a[0];
min = a[0];
for (j= 1 ; j<n; j++)
{
 if (max<a[j])

 {
    max = a [j];
 }
 if (min > a[j])
 {
    min = a[j];
 }
}
cout <<"The maximum element in the given array is: "<<max<<endl;
cout << " The minimun element in the array is: "<<min<<endl;
return 0;

}

//Search element
#include<iostream>
using namespace std;
int main()
{
     int n, i, j, s, c = 0, flag = 0;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}
cout << "Enter an element to be searched in an array: ";
    cin >> s;
for (j= 0 ; j<n; j++)
{
    if ( a[j]==s)
    {
cout<< "The element"<<" "<< s<< " " << "is present at location: "<<j<<endl;
c++;
flag =1;
    }
}

if( flag ==0)
{
    cout<< "The element"<< " "<< s << " "<< "is not present in the given array";
}
else
{
    cout << "The element" << " "<< s << " "<< "occurs"<< " "<< c << " "<< "times.";
}
return 0;
}
//USER INPUT
#include <iostream>
using namespace std;
int main()
{
    char s[]= "Parth";
    cout<<s<<endl;
    return 0;
}


//CONCATENATION
#include<iostream>
using namespace std;
int main() 
{
    string name("Parth");
    string surname("Borikar");
    name.append(surname);
    cout<<name<<endl;
}


//REVERSE STRING
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
int main()
{
string a= "Parth";
reverse(a.begin(), a.end());
cout<<"reverse string is:"<<a<<endl;
return 0;
}

//PALINDROME
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
int main() 
{
    string s1, s2;
    cout << "Enter a word to check";
    cin>>s1;
    s2=s1;
    reverse(s1.begin(), s1.end());
    if (s2==s1) 
    {
        cout<<"Yes! It is a palindrome";
    }
    else cout<<"No! It is not a palindrome";
}

```
# Output
1.) Array
![image](https://github.com/user-attachments/assets/f4dc76e5-e462-4e62-be30-483044553526)


2.) Reverse array
![image](https://github.com/user-attachments/assets/a12a2bb5-dfb3-4dc5-aeff-953bf3be6c35)


3.) Sum and average
![image](https://github.com/user-attachments/assets/08226f07-4e86-4b6c-b20a-d390c40c5c13)


4.) Maximum and minimum
![image](https://github.com/user-attachments/assets/9b544e22-b701-471f-88cc-d7ee4fcae4d9)


5.) Search element
![image](https://github.com/user-attachments/assets/9060d6f7-9138-4598-b2a6-7758d0db2790)

6.) USER INPUT
![image](https://github.com/user-attachments/assets/3c251893-1635-4479-babb-325afb9ea88b)


7.) CONCATENATION
![image](https://github.com/user-attachments/assets/0b336c15-4fb8-4985-87ce-c68613294876)


8.) REVERSE STRING
![image](https://github.com/user-attachments/assets/f5d46e1f-cfc3-4242-92f0-d37e2f86bb2c)


9.) PALINDROME
![image](https://github.com/user-attachments/assets/d28d19a3-94f4-4495-aca1-60b772bcf968)


# Conclusion

We learnt to create an array and operate it. 

We learnt to search element in the array and getting the sum and average of the elements.

We learnt to do concatenation of strings, making and checking palindromes, reversing the string in c++..
