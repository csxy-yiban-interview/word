#include <stdio.h>
#include <string.h>

 int main(void) 
 {
 	char ch[100];//字符数组 
	char t;//临时字符 
	int len;//保存字符长度 
	printf("Enter a string:");
	fgets (ch, 99, stdin);//获取，放到ch，标准输入 
    printf(ch);
	len = strlen(ch);//长度获取 
	for (int i = 0; i<len/2; i++) //for循环反转 
	{
		t=ch[i];
		ch[i]=ch[len-1-i];
		ch[len-1-i]=t;
		
		
		
	}
	printf("After:");
	printf(ch);
 	return 0;
 	
 	
 	
 }
