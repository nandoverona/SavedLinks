# Saved Links - References

## **Databases**

**General**
- Basics Of Consistency And Locking In Databases: https://recepinanc.com/Basics-of-Consistency-and-Locking-in-Databases/

## **Benchmarking**

**Tools**
- HammerDB https://www.hammerdb.com
  - How many warehouses to create for the TPROC-C test: https://www.hammerdb.com/docs/ch03s07.html
    - Important take away here, if IO is not important in your test, choose number of warehouses bigger than max number of virtual users if possible.
    
       *Also with the home warehouse chosen at random it should be clear that number of warehouses should be configured so that when the maximum number of virtual users that you will run are configured there is a good chance that the selection of a home warehouse at random will be evenly distributed across the available warehouses with one or possibly 2 virtual users selecting the same home warehouse at random but not more.*
       
       *Typically an option of 4 to 5 warehouses per virtual user would be a minimum value to ensure an even distribution of virtual users to warehouse. Therefore for the 100 virtual users 400 to 500 warehouses should be a minimum to be configured.*
 
  - HammerDB Market Published Benchmarks: https://www.hammerdb.com/benchmarks.html
  
- Sysbench
- PGBench (PostgreSQL specific)
