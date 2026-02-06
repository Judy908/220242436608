TO GENERATE A FREQUENCY ITEM GIVEN min_support=40%


step1: To calculate the mean support count

   given; total number of transactions, n=7
   
          min_support= 40% 0r 0.4
          
    then, 
    
         min_support_count=n*min_support_thredhold
         
                          = 7*0.4
                          
                          =2.8
                          
          Mean support count is approximated to 3.

          

step2:To generate frequent 1-item sets, L1

      -Counting the occurances of each single item in the transactions
      
     bread: 6
     
     milk: 6
     
     chips: 2
     
     mustard: 2
     
     beer: 4
     
     diaper: 5
     
     eggs: 1
     
     coke: 3
     
          items with count less than 3 are discarded
          
          L1= {{Bread},{Milk},{Beer},{Diaper},{Coke}}

          

step3: To generate frequent 2-items sets, L2

- Will be generated from the L1 and their support counts are calculated
  
- The sets with less than 3 counts will be discarded
  

{Bread,Milk}: 5

{Bread, Beer}: 3

{Bread, Diaper}: 4

{Bread,Coke}: 2

{Milk, Beer}: 2

{Milk, Diaper}: 5

{Milk, Coke}: 3

{Beer, Diaper}: 4

{Beer,Coke}: 2

{Diaper,Coke}: 3

 Therefore; L2= {{Bread,Milk},{Bread, Beer},{Bread, Diaper},{Milk, Diaper},{Milk, Coke},{Beer, Diaper},{Diaper,Coke}}



 step4: To generate the frequent 3-item sets, L3

 - This will be generated from L2 where their support counts
   
   {Bread,Milk,Diaper}: 4
   
   {Bread, Beer, Diaper}: 3
   
   {Milk,Diaper,Coke}: 3
   
   Therefore; L3= {{Bread,Milk,Diaper},{Bread, Beer, Diaper},{Milk,Diaper,Coke}}.
   
- since no 4-item sets the process stops.

  

   GENERALLY;
  
   The frequent item sets with minimum supoortof 40% are:
  

   1-item sets: {{Bread},{Milk},{Beer},{Diaper},{Coke}}
  
   2-item sets: {{Bread,Milk},{Bread, Beer},{Bread, Diaper},{Milk, Diaper},{Milk, Coke},{Beer, Diaper},{Diaper,Coke}}
  
   3-item sets: {{Bread,Milk,Diaper},{Bread, Beer, Diaper},{Milk,Diaper,Coke}}



  
          

