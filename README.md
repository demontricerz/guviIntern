# Help Peter to Recreate Cap's Shield
    Help Peter Parker to Recreate Captain America's Shield.

## Problem Statement
> Its Becoming the End of the **End Game** , Our Superheros were Ending their Mission of End Game with **Sacrifice of Mr Tony Stark**. 
>
> During the End Game **Captain America's Shield has been Destroyed by Thanos**. Mr **Peter Parker** an Young Scientist Discovered the formula for **Vibranium** *(A Material Used to Create Cap's Shield)*. 
>
> He has Numerous amount of **Phase 1** of Vibranium
>
> To Create the Shield He Needs to Produce **N**th Phase of Vibranium. 
>
> **Refination** is the Process where Vibranium in **Phase A** transforms to **Phase B** with some **Cost** of **C**.
>
> Help Peter to Find the **Minimum Cost** which is enough to Refine from **Phase 1** to Phase **N**
>

# Input Format

* First Line of the Input Consists of an **Integer N** Denotes **Final Phase**, where Phases of Vibranium ranges from 1 to **N**.
* Second Line of the Input Consists of an **Integer T** Denotes **No of Transformations** is Possible.
* Next **T Lines** Have **3 Space Separated Integers**
  - **SP** Denotes **Starting Phase**,
  - **EP** Denotes **Ending Phase** ,
  - **C** Denotes **Cost for transition**.

# Output Format

* Output needs to be in a Single line of **INTEGER** which is minimum cost required for refining Vibranium Phase **N**. 


# Constraints

- **2 < N <= 100**
- **N-1 < T < N^2**
- **1 < SP,EP <= N**
- **0 < C <= 10^6**


# Sample Input and Output 1
### Input

    3                  # Number of Phases It Contains
    3                  # Number of Transformations Possible
    1 2 5              # SP=1  EP=2 and C=5%
    1 3 7              # SP=1  EP=3 and C=7%
    2 3 5              # SP=2  EP=3 and C=5%

### Output

    7

### Explanation

N=3

Initial Phase | Ending Phase | Wastage
--- | --- | ---
 1 |	2 | 5
 1 |	3 | 7
 2 |	3 | 5
    # Visualisation
    
    
    		|1|
		  5    /   \  7
		      /     \
		    |2|-----|3|
		    	5
    



To get a Complete Transformation from 1 to 3 we can have two Possible paths.
* 1 --> 3  
    * **Total Cost = 7**

* 1--> 2 --> 3  
    * For Transformation 1 -> 2
    * Cost = 5
    * For Transformation 2 -> 3
    * Cost = 5
    * **Total Cost = 10**

* 1--> 3 Gives Minimum Cost
* So Output is **7**


## Test Cases for Evaluations

####Case #1

    6
    14
    1 2 5
    1 3 9
    2 3 1
    2 4 7
    3 5 4
    4 5 2
    5 6 11
    4 6 4
    3 4 6
    1 4 8
    2 5 11
    3 6 11
    2 6 35
    1 5 23
    
#### Output #1

    12
    
#### Input #2
    10
    9
    1 2 10
    2 3 10
    3 4 10
    4 5 10
    5 6 10
    6 7 10
    7 8 10
    8 9 10
    9 10 10

###Output #2
    90
