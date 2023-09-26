#include <stdio.h>
#include <stdlib.h>
#include <time.h>

 int
flipCoin ()
{
  
  // Generate a random number between 0 and 1
  int result = rand () % 2;
  
 
   // Return 0 for heads and 1 for tails
    return result;

}


 
int
main ()
{
  
   // Seed the random number generator with the current time
    srand (time (0));
  
 
  // Flip the coin and print the result
  int coin = flipCoin ();
  
if (coin == 0)
    {
      
printf ("Heads\n");
    
}
  else
    {
      
printf ("Tails\n");
    
}
  
 
return 0;

}


