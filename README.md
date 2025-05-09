# cpt-9
code::1
'''write a program to read a character untill * is emtered.
count the no.of uppercase , lowercase, and no's entered by the user'''


ch = input("enter any character:")
n=u=l=0
if ch>='0' and ch<='9':
    n+=1
elif ch>='a' and ch<='z':
    l+=1
elif ch>='A' and ch<='z':
    u+=1
while ch!='*':
    ch = input("enter any character:")
    if ch>='0' and ch<='9':
        n+=1
    elif ch>='a' and ch<='z':
        l+=1
    elif ch>='A' and ch<='z':
        u+=1
print("lowercase char:",l)
print("uppercase char:",u)
print("number char:",n)

output:
enter any character: h
enter any character: 5
enter any character: l
enter any character: 4
enter any character: D
enter any character: Q
enter any character: *
lowercase char: 2
uppercase char: 2
number char: 2
code::2
# simple for loop (string)
str= 'cheetah'
for i in str:
    print(i, end=' ')

output::
c h e e t a h
code::3
# list of strings
s= ['cat','dog','fish']
for pet in s:
    print(pet)

  output::
  cat
  dog
  fish
code:4
# for with in range
n=int(input("enter the value of n"))
for i in range(21, n+1,2):
    print(i, end=' ')
output::5
enter the value of n 50
21 23 25 27 29 31 33 35 37 39 41 43 45 47 49 
code::5
# for with in range
n=int(input("enter the value of n"))
for i in range(1, n+1):
    print(i, end=' ')
for i in range(n, 0, -2):
    print(i,end=' ')
  output::
  enter the value of n 10
1 2 3 4 5 6 7 8 9 10 10 8 6 4 2 

code::6
'''code for printing multiplication table of n,where n is enterd by the user
input:
enter any number:2
output:
multiplication table of 2
**************************
2 X 0 = 0
2 X 1 = 2
2 X 2 = 4
.
.
'''
n=int(input("enter any number:"))
e=int(input("enter any number:"))
print("Multiplication table of",n)
print("********************")
for i in range(1,e+1,1):
    print(f"{n} X {i} ={n*i}")
output::
enter any number: 2
enter any number: 10
Multiplication table of 2
********************
2 X 1 =2
2 X 2 =4
2 X 3 =6
2 X 4 =8
2 X 5 =10
2 X 6 =12
2 X 7 =14
2 X 8 =16
2 X 9 =18
2 X 10 =20
code::7
# program to display all the leap years from 1900,2101
st= int(input("Enter the starting year:"))
ed= int(input("Enter the ending year:"))
for i in range(st, ed+1):
    if i%4==0:
        print(i,end=' ')
output::
Enter the starting year: 1900
Enter the ending year: 2101
1900 1904 1908 1912 1916 1920 1924 1928 1932 1936 1940 1944 1948 1952 1956 1960 1964 1968 1972 1976 1980 1984 1988 1992 1996 2000 2004 2008 2012 2016 2020 2024 2028 2032 2036 2040 2044 2048 2052 2056 2060 2064 2068 2072 2076 2080 2084 2088 2092 2096 2100 
code::8
# series 1+1/2*2+1/3*3....1/n*2
n = int(input("enter the value of n:"))
s=0.0
for i in range(1, n+1):
    a=1/(i**2)
    s=s+a
print(s)
output::
enter the value of n: 5
1.4636111111111112
code::9
# program to build calendar of a month
import calendar
year=int(input("Enter year:"))
month= int(input("Enter month:"))
cal=calendar.month(year,month)
print(cal)
output::
Enter year: 2023
Enter month: 12
   December 2023
Mo Tu We Th Fr Sa Su
             1  2  3
 4  5  6  7  8  9 10
11 12 13 14 15 16 17
18 19 20 21 22 23 24
25 26 27 28 29 30 31
code::10
# calendar
mdays=31
sday=0
print(" Sun  Mon  Tue  Wed  Thu  Fri  Sat")
for _ in range(sday):
    print("  ",end=' ')
for days in range(1, mdays+1):
    print(f"{days: >3} ", end=' ')
    if (sday+days) %7==0:
        print()
output::
Sun  Mon  Tue  Wed  Thu  Fri  Sat
  1    2    3    4    5    6    7  
  8    9   10   11   12   13   14  
 15   16   17   18   19   20   21  
 22   23   24   25   26   27   28  
 29   30   31  

