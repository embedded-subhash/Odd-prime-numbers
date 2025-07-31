  #include<stdio.h>
int check_prime (int v)
{
for(int i=2;i<v;i++)
{
if(v%i==0)
return 0;
}
return 1;
}
int check_odd(int v)
{
int temp=v,d;
while(temp)
{
d=temp%10;
if(d%2!=0)
return 1;
temp/=10;
}
return 0;
}
int main()
{
for(int  i=100; i<180;i++)
if(check_prime(i))
if(check_odd(i))
printf("%d".,i);
}
