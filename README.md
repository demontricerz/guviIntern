# Help Peter to Recreate Cap's Shield
    Help Peter Parker to Recreate Captain America's Shield.

## Problem Statement
> Its Becoming the End of the **End Game** , Our Superheros were Ending their Mission of End Game with **Sacrifice of Mr Tony Stark**. 
>
> During the End Game **Captain America's Shield has been Destroyed by Thanos**. Mr **Peter Parker** an Young Scientist Discovered the formula for **Vibranium** *(A Material Used to Create Cap's Shield)*. 
>
> he has Numerous amount of **Phase 1** of Vibranium
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


