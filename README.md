# saving-an-important-element-in-life
#include <stdio.h>
int save(int n){
    
    if(n==0){
        return 0;
    }
    else{
       return (n+save(0.02*n));
    }
    
}
int main() {
  int i,j,a;
  printf("Enter amount you want to save:");
  scanf("%d",&i);
  printf("\n2 percent of interest will be added to your amount\n");
  
  int result=save(i);
    printf("\nAmount you save will become=%d",result);
    return 0;
}
