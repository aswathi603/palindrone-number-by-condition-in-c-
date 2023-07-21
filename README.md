# palindrone-number-by-condition-in-c



        #include <stdio.h>
        int main() {

        /* Enter your code here. Read input from STDIN. Print output to STDOUT */
        int a,n;
        int s=0,c=0;
        scanf("%d",&n);
        a=n;
        while(a!=0)
        {
          int r=a%10;
          s=(s*10)+r;
          a=a/10;
        }
        for(int i=1;i<=n;i++)
        {
          if(n%i==0)
          {
              c=c+1;
          }
        }
        if (c==2 && s==n)
        {
          printf("YES");
        }
        else
        {
          printf("NO");
        }
        return 0;
        }
