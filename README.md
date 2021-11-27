# Calculate-total-runs-scored-by-Team-in-Cricket
#include<stdio.h>
struct player
{
     char name[20];
     int runs;
};
int main()
{
     int i,s=0;
     struct player a[11]; //a[11] - no. of players
     printf("Enter Name of Player Runs Scored \n");
     printf("---------------------------------------------\n\t");
     for(i=0;i<=10;i++)
     {
          scanf("%s",a[i].name);
          scanf("%d",&a[i].runs);
          printf("\t");
     }
     for(i=0;i<=10;i++)
          s=s+a[i].runs;
     printf("\n---------------------------------------------\n");
     printf("Total Runs Scored by Team: %d",s);
     return 0;
}

/* Output

Enter Name Of Player          Runs scored
--------------------------------------------
Rohit Sharma                    60
shikhar Dawan                   50
Virat Kohli                    111
suryakumar yadav                30
Rishab pant                     10
Hardik Pandya                   15
Ravindra Jadeja                 55
Krunal Pandya                   20
Bhuvneshwar Kumar                5
Jasprit Bumrah                  10
Mohammed Shami                  12
--------------------------------------------
Total Runs=                    378             */
