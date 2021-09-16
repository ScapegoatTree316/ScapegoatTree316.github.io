---
title: CF518B Tanya and Postcard 题解
date: 2021-09-16 20:23:37
tags:
---

## 思路

- 由于题目要求匹配大小写，我们要将大小写分开存放。
- 统计$s,t$的每个字母大小写个数。
- 由于要求“耶”尽可能多，所以尽可能匹配大小写。
- 将大小写尽可能匹配后，剩下的只有可能是“哎呦”，因此对于$s,t$​中剩余的字母，取每个字符不区分大小写后的最小值，加和即可。

<!-- more -->

## 代码
```cpp
#include<bits/stdc++.h>
#define int long long
namespace SGT
{
	char getc(){return getchar();}
	void putc(char ch){putchar(ch);}
	int read(){int mk=1,x=0;char ch=getc();while(ch!='-'&&(ch<'0'||ch>'9'))ch=getc();if(ch=='-')mk=-1,ch=getc();while('0'<=ch&&ch<='9')x=(x<<1)+(x<<3)+(ch^48),ch=getc();return x*mk;}
	void write(int x,char ch){char cc[100000];int t=0;if(x==0)putc('0');if(x<0) putc('-'),x=-x;while(x){cc[++t]=char(x%10+48);x/=10;}for(int i=t;i>=1;i--)putc(cc[i]);putc(ch);}
	void write(char str[],char ch){for(int i=0;i<strlen(str);i++)putc(str[i]);putc(ch);}
	void write(char wr,char ch){putc(wr);putc(ch);}
	int max(int a,int b){return (a>b?a:b);}
	int min(int a,int b){return (a<b?a:b);}
}
using namespace SGT;
char s[200010];
int t1[200],t2[200],tt1,tt2,ans1,ans2;
signed main()
{
	char ch=getc();
	while(ch!='\n')
	{
		t1[ch-'A']++;
		ch=getc();
	}
	ch=getc();
	while(ch!='\n')
	{
		t2[ch-'A']++;
		ch=getc();
	}
	for(int i=0;i<=25;i++)
	{
		if(t1[i]>t2[i]) t1[i]-=t2[i],ans1+=t2[i],t2[i]=0;
		else t2[i]-=t1[i],ans1+=t1[i],t1[i]=0;
	}
	for(int i1=0;i1<=25;i1++)
	{
		int i=i1+'a'-'A';
		if(t1[i]>t2[i]) t1[i]-=t2[i],ans1+=t2[i],t2[i]=0;
		else t2[i]-=t1[i],ans1+=t1[i],t1[i]=0;
	}
	for(int i=0;i<=25;i++)
	{
		tt1=t1[i]+t1[i+'a'-'A'];
		tt2=t2[i]+t2[i+'a'-'A'];
		ans2+=min(tt1,tt2);
	} 
	write(ans1,' ');
	write(ans2,'\n');
	return 0;
}
```
