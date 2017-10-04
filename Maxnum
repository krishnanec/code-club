#include <stdio.h>

int main(void) {
    int i,n,max=0,in=0,ex=0,p,l;
    scanf("%d",&n);
    int a[100];
    for(i=0;i<n;i++)
     scanf("%d",&a[i]);
    l=n;
    while(l)
    {   
        max=0;
        for(i=0;i<n;i++)
        if(max<a[i])
        {
            max=a[i];
            p=i;
        }
        l--;
        in=in+max;
        a[p]=-1;
        if((p-1)!=-1&&!(a[p-1]<0))
        {   l--; 
            ex=ex+a[p-1];
            a[p-1]=-1;
        }
         if((p+1)!=n&&!(a[p+1]<0))
        { l--; 
            
            ex=ex+a[p+1];
            a[p+1]=-1;
            
        }
        
        
    }
    printf("%d",(in>ex)?in:ex);
    
	return 0;
}
