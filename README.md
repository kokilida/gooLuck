main() {

printf " Please print an array-finish with -1\n"
new j=0
new a[100]
new b[]=[1,2,3,4,5]
new size=5;
for (;;) 
{
new check=getvalue()
if (check!=-1){
a[j]=check
j=j+1
}
else {
break
}
}


new sumA=sumIt(a,j)
printf "The sum is %d\n",sumA

new sumB=sumIt(b,size)
printf "The sum is %d\n",sumB
}

sumIt(array[],arraySize)
{

new sum=0

for (new i=0;i<arraySize; i++){
sum=sum+ array[i]
}
printf "%d\n",sum
return sum
}


***************

main()
{

for(new i=0;i<2;i++){
for(new j=2;j>=0;j--){
if(i==j) break
printf "i= %d  j=  %d\n" ,i,j
}
}
}

*******************


main()
    {
    printf "Please type the string \n"
	new str[100]
    getstring str, sizeof str, .pack = false
  if  (isCapital(str))
    printf "Capital\n"
	else
	 printf "Not Capital\n"
  

    printf "The string is: \"%s\"\n", str
    }

isCapital(string[])
    {
    new index = 0;

        if ('a' <= string[index] <= 'z')
      return false
        else if ('A' <= string[index] <= 'Z')
          return true	  
		 else
		return false  
    }

