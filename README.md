
Hello!Everyone!My name is"Li Haoxia". I from Shanxi Datong.I am a digital media technology major.<br>
I love life and I love code.My life is rich ang colorful,I like watching TV plays and studying.<br>
I want to join you to learn a lot of professional computer knowledge,access to many competition<br>
channels and opportunities.I need to improve my ability ang exercise my thinking.Maybe my ability <br>
is not outstanging,but I want to try to make myself better.I  hopeI can be recognized. <br>

![image](https://github.com/Emconnc/lihaoxia/blob/main/%E5%8C%97%E5%8D%B0_20220920134337.jpg)
2.1冒泡算法的具体过程：<br>
第一步：比较n-1轮数字大小，每一个数字比较n-1-i次<br>
第二步：依次比较相邻位置前一个数字与后面数字的大小，如果前面数字比后面数字大就更换位置<br>
第三步：重复前面步骤，直到排序完成<br>
#include<stdio.h><br>
int main()<br>
{<br>
	int n[10]={2,6,8,4,9,7,1,3,10,5};<br>
	int i,j,k;<br>
	for(i=0;i<10-1;i++)//进行n-1轮比较<br>
	{<br>
		for(j=0;j<10-1-i;j++)//每一个循环比较前n-1-i个数字，不用比较已经比较完的前i个数字<br>
		{<br>
			if(n[j]>n[j+1])//如果前面数字比后面大，前后换位置<br>
			{<br>
				k=n[j];<br>
				n[j]=n[j+1];<br>
				n[j+1]=k;<br>
			}<br>
		}<br>
	}<br>
	for(i=0;i<10;i++)//依次输出已经排序好的数字<br>
		printf("%d ",n[i]);<br>
	return(0);<br>
}<br>
