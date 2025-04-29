# cs6700---reinforcement-learning-solved
**TO GET THIS SOLUTION VISIT:** [CS6700 – Reinforcement Learning Solved](https://www.ankitcodinghub.com/product/cs6700-reinforcement-learning-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;110514&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6700 - Reinforcement Learning Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Programming Assignment 1

1 Environment Description

This exercise aims to familiarize you with two popular Temporal Difference Learning algorithms: SARSA and Q-Learning. You will solve several variants of the Grid World problem (a sample world is shown in Figure 2).

This is a grid world with 4 deterministic actions (‘up’, ‘down’, ‘left’, ‘right’). The agent transitions to the next state determined by the direction of the action chosen with a probability of p ∈ [0,1]. We also define a parameter called b ∈ [0,1]. Consider the direction of the action chosen as the agent’s “North”. For example, if the action is ‘left’, it is the agent’s North, and the agent’s East would be the direction of the action ‘up’. Figure 1 provides an illustration of the same. The agent transitions to the state West of the chosen action with probability (1−p)×b, and to the East of the chosen action with probability (1−p)×(1−b).

The dimensions of the grid are 10 × 10. The following types of states exist:

• Start state: The agent starts from this state.

• Goal state: The goal is to reach one of these states. There are 3 goal states in total.

• Obstructed state: These are walls that prevent entry to the respective cells. Transition to these states will not result in any change.

• Bad state: Entry into these states will incur a higher penalty than a normal state.

• Restart state: Entry into these states will incur a very high penalty and will cause agent to teleport to the start state without the episode ending. Once the restart state is reached, no matter what action is chosen, it goes to the start state at the next step. • Normal state: None of the above. Entry into these states will incur a small penalty.

Rewards: -1 for normal states, -100 for restart states, -6 for bad states, +10 for goal states.

Figure 1: The intended direction of the action chosen is considered as ‘North’

Additional Information

Figure 2: An example grid world with start position (0,4)

2 Tasks

• Implement SARSA and Q-Learning.

• For each algorithm, run experiments with wind=False and wind=True; two different start states: (0,4), (3,6); two values of p (1.0, 0.7); and two types of exploration strategies (ϵ-greedy and softmax), making it 16 different configurations in total.

• For each of the 16 configurations, determine the best set of hyperparameters (ϵ in ϵ-greedy exploration, temperature β in softmax exploration, learning rate α, and discount factor γ) and plot the following:

1. Reward curves and the number of steps to reach the goal in each episode (during the training phase with the best hyperparameters).

2. Heatmap of the grid with state visit counts, i.e., the number of times each state was visited throughout the training phase.

3. Heatmap of the grid with Q values after training is complete, and optimal actions for the best policy.

For each of the algorithm, provide a written description of the policy learnt, explaining the behavior of the agent, and your choice of hyperparameters. This description should also provide information about how the behavior changes with and without the wind, for different levels of stochasticity and for different start states.

Figure 3 summarizes how you can structure your report.

Figure 3: The report can be organized in this manner

3 Submission Instructions
