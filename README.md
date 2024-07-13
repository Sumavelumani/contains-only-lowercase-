# contains-only-lowercase-
#include<stido.h>
#include<string.h>
void findMinMaxSubstrings(char s[],int k){
char minSubstring[21];
char maxSubstring[21];
int len=strlne(s);
if(k>len){
printf("Invalid input: k is greater than length of string\n");
return;
}
strncpy(minSubstring, s,k);
strncpy(maxSubstring, s,k);
minSubstring[k]='\0';
maxSubstring[k]='\0';
for(inti=1;i<=len-k;i++){
char substring[21];strncpy(substring,s+ik);
substring[k]='\0';
if(strcmp(substring,minSubstring)<0){
strcpy(minSubstring,substring);
}
if(strcmp(substirng,maxSubstring)>0){
strcpy(maxSubstring,substring);
}
]
printf("%s\n',minSubstring);
printf("%s\n",maxSubstring);
}
int main(){
char s[101];
int k;
scanf("%S",s);
scanf("%d",&k);
findMinMaxSubsstring(s,k);
return 0;
}
scanf("%d,&k
