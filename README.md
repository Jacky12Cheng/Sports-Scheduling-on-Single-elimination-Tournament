# Sports-Scheduling-on-Single-elimination-Tournament

## **Problem Description**

Exciting sports events always can gather people's hearts. So whether the good matchup or not is important. This why we want to solve this problem. However, many factors would affect the popularity of the game. The love of audience and box office are supplementary to each other. In this problem we consider the following factors:
- Number of audience (box office)
- Venue
- The strength of the team

The objective function is to **maximize the popularity and box office of the game.** The box office will be affected by different venues.

The following figure shows the result we want to get. English letters in brackets represent the venue. So we will decide the matchup and venue simultaneously in every single game session.

## **Problem Assumption**

There are some assumptions about this project as the following points.
- In this project, we focus on the single-elimination tournament. It means that if a team once failed, the team will be eliminated in the same time.
- We decide whether to win or lose based on team strength, the stronger team always got the victory of the matchup.
- Box office will vary according to different matchups and venues; I determine the value by a discrete uniform distribution ( U(1,20) ).
- The venues should not be repeated in the preliminary round and final round. The preliminary round and final round will be explained in the following context.
![This is an image](https://github.com/Jacky12Cheng/NBA-Industry-Chain-Database-Management-System-with-GUI/blob/main/ER_Diagram_and_Relation_Schema/ER-diagram.png)

## **Integer Programming Approach**
- Given Data

There are some data is given in this project. One is box office data, it is a three-dimension data set which is based on different matchups and venues.

The other one is the team strength table. We determine which will win by using the table.

- Objective function
Maximize the total box office income

I will explain the variables in the function later.

- Variable & Parameter Definition

- Constraints
  - Ubar Constraints
  To simply our problem, we construct the variable u ̅_ijp. 
  
  - Advance Constraints
We decide whether to win or lose based on team strength.
 
 
  - Venue Constraints

  - Competition system Constraints
 
  - Objective function Constraints

## **Computational Results**

The results are shown in the following figures. We got the variables u and v about the matchup and venue in the every game session.

Then we did some comparison between different numbers of teams and venues as follows.

## **Conclusions**

Based on the computational results, increasing the number of venue choices will not have much impact on the solution time. However, increasing the number of teams by a factor of two will lead to an exponential increase in solution time. So we need to revise our integer programming model to reduce the use of binary variables.
