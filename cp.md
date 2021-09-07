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

### Interactive Problem:
![image](https://user-images.githubusercontent.com/89128563/132125179-c8369aa8-79c4-4889-ae08-c575e8ef4682.png)
![image](https://user-images.githubusercontent.com/89128563/132125193-0035474a-b896-4301-ae01-ba8e09512ce6.png)
![image](https://user-images.githubusercontent.com/89128563/132125234-9d1c6427-50c6-4d11-87f6-a0e70884cf05.png)
![image](https://user-images.githubusercontent.com/89128563/132125257-07f3dfc2-62bb-4330-b4cf-bdc7e532271d.png)
![image](https://user-images.githubusercontent.com/89128563/132125286-4b613be2-2f5b-4691-bcbc-00ba1210cabe.png)
![image](https://user-images.githubusercontent.com/89128563/132125304-c7ebee8e-d68e-4fa0-8b44-5d6a950642fc.png)
![image](https://user-images.githubusercontent.com/89128563/132125319-e16b6a23-ade4-4881-8c87-5377ee153e8d.png)
 ![image](https://user-images.githubusercontent.com/89128563/132125404-46c79651-d2bb-42e7-bcdf-1759cebf0bd5.png)
 
 ***************
 
 input is given according to our query.
 ![image](https://user-images.githubusercontent.com/89128563/132125560-1daf788a-98d2-42bc-9f2d-4d3d1b31ad20.png)
 ![image](https://user-images.githubusercontent.com/89128563/132125675-bd13dc18-feac-4340-b75a-8fbe984a5f99.png)

 ![image](https://user-images.githubusercontent.com/89128563/132125693-f73cd043-ccb7-42fe-8644-993bedbefb49.png)
logn query
  
![image](https://user-images.githubusercontent.com/89128563/132125746-9884e00c-1b83-4830-bc04-415a6ec0843f.png)


## Digit-DP
- another type of dp
- problem type 1: find out the count of integers x such that  0<=x<=R which obey the functinon f(x)
- problem type 2: how many no x are ther in the range [L,R] inclusive which obey the funciton f(x) wher f(x) is binary fucntin .
-brute force: iterate form l to r and check f(x) wheather f(x) is true or not 
-tc:o((r-l)*T) r=1e9 or r=1e18 or r=1e1000
-we can not solve such problem by iterating to all no. here comes digit dp


sol-problem-1:
- S(R)-count of no in the range [L,R] which obey the function F(x).
![image](https://user-images.githubusercontent.com/89128563/132180889-e6bdd415-3074-4926-b6f8-731143cd7a13.png)
- if we able to find S(R) then we can find S(L-1) then S(L,R)=S(R)-S(L-1)
![image](https://user-images.githubusercontent.com/89128563/132181193-4e823fdf-a72f-49b3-9a38-c0f04cc23343.png)
- brute force: iterate 
![image](https://user-images.githubusercontent.com/89128563/132181462-52632c7c-8c7c-4728-a5b8-536e44cdba85.png)
![image](https://user-images.githubusercontent.com/89128563/132181555-b65ff0a2-ed7b-4495-96a0-91528b49bb2f.png)
- 





