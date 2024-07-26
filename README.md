# Star-rectangle-pattern-for-n-5

Output :- 

*********
**** ****
***   ***
**     **
*       *
**     **
***   ***
**** ****
*********


## Python code for above pattern

## for upper part
n = int(input())
for i in range(n,0,-1):
    print('*'*(i),end="")
    print(" "*(2*(n-i)-1),end="")  ## for spaces
    if(i==n):
        print('*'*(i-1))
    else:
        print("*"*i)

## for lower part
for i in range(2,n+1):
    print('*'*i,end="")
    print(" "*(2*(n-i)-1),end="")
    if(i==n):
        print('*'*(i-1))
    else:
        print("*"*i)
