---
title: CF534C Polycarpus' Dice 题解
date: 2021-09-16 20:22:11
tags:
---

## 更正题意

- 要求输出的是每个色子不能达到要求点数的个数。

<!-- more -->

## 思路

- 对于一个色子，我们先求出其他色子可以掷出的范围，那么我们就能得到这个色子所可能掷出的范围，这样将这个范围减去就可以求出答案了。

## 代码

```cpp
#include<bits/stdc++.h>
#define int long long
namespace SGT
{
	char getc(){return getchar();}
	void putc(char ch){putchar(ch);}
	int read(){int mk=1,x=0;char ch=getc();while(ch!='-'&&(ch<'0'||ch>'9'))ch=getc();if(ch=='-')mk=-1,ch=getc();while('0'<=ch&&ch<='9')x=(x<<1)+(x<<3)+(ch^48),ch=getc();return x*mk;}
	void write(int x,std::string ch){char cc[100000];int t=0;if(x==0)putc('0');if(x<0) putc('-'),x=-x;while(x){cc[++t]=char(x%10+48);x/=10;}for(int i=t;i>=1;i--)putc(cc[i]);if(ch.size()>0)putc(ch[0]);}
	void write(char str[],std::string ch){for(int i=0;i<strlen(str);i++)putc(str[i]);if(ch.size()>0)putc(ch[0]);}
	void write(char wr,std::string ch){putc(wr);if(ch.size()>0)putc(ch[0]);}
	int max(int a,int b){return (a>b?a:b);}
	int min(int a,int b){return (a<b?a:b);}
	int gcd(int a,int b){int r;while(b>0){r=a%b;a=b;b=r;}return a;}
}
using namespace SGT;
int n,k,a[200010],sum;
signed main()
{
	n=read();
	k=read();
	for(int i=1;i<=n;i++)
	{
		a[i]=read();
		sum+=a[i];
	}
	for(int i=1;i<=n;i++)
	{
		int ans=0;
		int minn=n-1;
		int maxx=sum-a[i];//其他色子的范围
		if(k-maxx>0) ans+=k-maxx-1;
		if(k-minn<=a[i]) ans+=a[i]-k+minn;
		write(ans," ");
	}
	return 0;
}


```
