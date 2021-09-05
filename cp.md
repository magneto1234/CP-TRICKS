# Stl


``` cpp
map_name.upper_bound(key)
 mp.insert({ 12, 30 });
mp.insert({ 11, 10 });
mp.insert({ 15, 50 });
mp.insert({ 14, 40 });
auto it = mp.upper_bound(11);
cout << "The upper bound of key 11 is ";
cout << (*it).first << " " << (*it).second << endl;
```
![image](https://user-images.githubusercontent.com/89128563/132104900-584a17b9-8371-4ccc-a007-97093076c53e.png)
![image](https://user-images.githubusercontent.com/89128563/132105030-3aa924c5-85d7-461c-bda9-5132d9a5a041.png)
- BITSET
- each position in bitset takes 1 bit wheraas in boolean array each position takes 8 bits
![image](https://user-images.githubusercontent.com/89128563/132105067-acfce0f3-07f1-446f-b712-ac23d04bead8.png)
``` cpp
bitset<10>bs
cout<<bs;//0000000000
******
bitset<10>bs(5);
cout<<bs; //0000000101
*****
bitset<10>bs("10011");
cout<<bs; // 0000010011
```
- accesign individual bits
``` cpp
bitset<10>bs("10011");
cout<<bs[0]; //1

```
![image](https://user-images.githubusercontent.com/89128563/132105220-fd4a5e30-fa3e-4d2f-b086-f5378b941c3d.png)
``` cpp
bitset<10>bs
bs[0]=1;
bs[2]=1;
cout<<bs;// 0000000101
******
bitset<10>bs
bs.set()
cout<<bs;// 1111111111
******
bitset<10>bs
bs.set(1);
cout<<bs;// 0000000010
****
bitset<10>bs
bs.set(0,1);
cout<<bs;// 0000000001

****
bs.reset() make all value to 0
bs.reset(1); //1111111101
******
bs.flip(1) flip 1st bit
*****
bitset<10>bs
bs.any()- retrn true if any of the bit is set it none set return false
cout<<bs.any();//false;
bs.count() return no of bits which are set

```
![image](https://user-images.githubusercontent.com/89128563/132105385-c82911e0-e9c9-476b-b404-5e86ed969c6a.png)
``` cpp
bitset<10>bs(5)
string st=bs.to_string();
cout<<st;
****
int x=bs.to_ulong();
cout<<x//5
*** long long x=bs.ullong();

****
bitset<10>bs(5);
bitset<10>st(6);
cout<<(st&bt);// 0000000100


```

##  next_permutation(), prev_permutation(), nth_element()

``` cpp
int ar[]={1,2,3};
123,132,213,231,312,321
next_permutation() return true or false if next greater perm exitst
cout<<next_permutation(ar,ar+3)<<endl;//1
 

```

