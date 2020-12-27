# Recreate Cap's Shield
    Help Peter Parker to Recreate Captain America's Shield.

## Problem Statement
> Its Becoming the End of the **End Game** , Our Superheros were Ending their Mission of End Game with **Sacrifice of Mr Tony Stark**. 
>
>During the End Game **Captain America's Shield has been Destroyed by Thanos**. Mr **Peter Parker** an Young Scientist Discovered the formula for **Vibranium** *(A Metal Used to Create Cap's Shield)*. 
>
>To Create the Shield He Needs to Produce Maximum Number of **Stable Phase** of Vibranium. 
>
>**Stable Phase** is Nothing But the Final **N** th Phase.
>
>**Refination** is the Process where Vibranium in **Phase A** transforms to **Phase B** with some Wastage of **Percentage P**.
>
>Help Peter to Find the **Maximum pounds of Stable Phase of Vibranium** we produce While Refining from **Phase 1** to Phase **N**
>

# Input Format

* First Line of the Input Consists of an **Integer N** Denotes **Final Phase**, where Phases of Vibranium ranges from 1 to **N**.
* Second Line of the Input Consists of an **Integer K** denotes **Amount of Phase 1 Vibranium** We have in **Pounds**.
* Third Line of the Input Consists of an **Integer T** Denotes **No of Transisions** is Possible.
* Each Line of the Following T lines Have **3 Space Separated Integers**
  - **SP** Denotes **Starting Phase**,
  - **EP** Denotes **Ending Phase** ,
  - **WP** Denotes **Waste Percentage**.

# Output Format

* Output needs to be in Single line of **Floating Value Limited Upto 3 Decimal Points** Denoting the **Amount of Stable Vibranium Produced** with **K** Pounds of Phase 1 Vibranium.


# Sample Input and Output 1
### Input

    3                  # Number of Phases It Contains
    150                # we have 150 Pounds of Vibranium 
    3                  # Number of Transitions Possible
    1 2 5              # SP=1  EP=2 and WP=5%
    1 3 7              # SP=1  EP=3 and WP=7%
    2 3 5              # SP=2  EP=3 and WP=5%

### Output

    2

### Explanation

N=3

Initial Phase | Ending Phase | Wastage
--- | --- | ---
 1 |	2 | 5%
 1 |	3 | 7%
 2 |	3 | 5%
    # Visualisation
    
    
    		|1|
		  5%   /   \  7%
		      /     \
		    |2|-----|3|
		    	5%
    



To get a Complete Transition from 1 to 3 we can have two Possible paths.
* 1 --> 3  
    * amoont = 150 - 150*(7/100)
    * amoont = 150 - 150*0.07
    * amoont = 150 - 10.5
    * amount = 139.5 Pounds

* 1--> 2 --> 3  
    * For Transition 1 -> 2
    * amoont = 150 - 150 * (5/100)
    * amoont = 150 - 150 * 0.05
    * amoont = 150 - 7.5
    * amount = 142.5 Pounds
    * For Transition 2 -> 3
    * amoont = 142.5 - 142.5 * (5/100)
    * amoont = 142.5 - 142.5 * 0.05
    * amoont = 142.5 - 7.125
    * amount = 135.375 Pounds.

* 1--> 3 Gives higher Amount
* So Output is 135.375 Pounds

