---
title: CF1360G A/B Matrix 题解
date: 2021-09-16 20:22:58
tags:
---

## 思路

- 首先判断“NO”，可以发现只有$n*a=m*b$是才会是“YES”。
- 接着，我们可以记录上一行到哪一位，这一行接着那一位往下构造，可以证明，这样每一列的1的个数最多差1，可以证明这样构造出来的答案正确。

<!-- more -->



如$n=3,m=6,a=2,b=1$时：
```
1 1 0 0 0 0
0 0 1 1 0 0
0 0 0 0 1 1
```
## 代码
```cpp
#include<bits/stdc++.h>
#define int long long
namespace SGT
{
	char getc(){return getchar();}
	void putc(char ch){putchar(ch);}
	int read(){int mk=1,x=0;char ch=getc();while(ch!='-'&&(ch<'0'||ch>'9'))ch=getc();if(ch=='-')mk=-1,ch=getc();while('0'<=ch&&ch<='9')x=(x<<1)+(x<<3)+(ch^48),ch=getc();return x*mk;}
	void write(int x,std::string ch){char cc[100000];int t=0;if(x==0){putc('0');return ;}if(x<0) putc('-'),x=-x;while(x){cc[++t]=char(x%10+48);x/=10;}for(int i=t;i>=1;i--)putc(cc[i]);if(ch.size()>0)putc(ch[0]);}
	void write(char str[],std::string ch){for(int i=0;i<strlen(str);i++)putc(str[i]);if(ch.size()>0)putc(ch[0]);}
	void write(char wr,std::string ch){putc(wr);if(ch.size()>0)putc(ch[0]);}
	int max(int a,int b){return (a>b?a:b);}
	int min(int a,int b){return (a<b?a:b);}
}
using namespace SGT;
int T,n,m,a,b,ans[100][100];
signed main()
{
	T=read();
	while(T--)
	{
		memset(ans,0,sizeof(ans));
		n=read(),m=read(),a=read(),b=read();
		if(n*a!=m*b)
		{
			write("NO","\n");
			continue;
		}
		write("YES","\n");
		int xb=1;
		for(int i=1;i<=n;i++)
			for(int j=1;j<=a;j++)
			{
				ans[i][xb++]=1;
				xb=(xb-1)%m+1;
			}
		for(int i=1;i<=n;i++)
		{
			for(int j=1;j<=m;j++)
				write(ans[i][j],"");
			write("","\n");
		}
	}
	return 0;
}

```
