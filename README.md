# **Assignment 1 - Deep Reinforcement Learning Course**

## **Overview**
This notebook is part of the first assignment for the Deep Reinforcement Learning (DRL) course. It implements a simplified grid-world environment modeled as a deterministic Markov Decision Process (MDP). The purpose of the notebook is to practice key reinforcement learning concepts, including state transitions, rewards, and termination conditions.


## **Instructor Information**
**Instructor:** Wiem Khlifi  
**Co-Instructors:** Imen Jendoubi, Oussama Mahfoudhi  




## **Tasks**
### **Completed Tasks**
1. **Initialization of Reward Table**  
   - Implemented the reward system for the grid-world.  
   - The agent receives:
     - **+100** for reaching the Goal (G).
     - **-100** for falling into the Hole (H).
     - **0** for all other transitions.

2. **Initialization of Transition Table**  
   - Defined all possible state transitions based on the agent's actions:
     - **Left, Down, Right, Up (0, 1, 2, 3)**.
     - Ensured correct transitions for terminal states (Goal and Hole).

3. **Agent Action Execution (`step` Function)**  
   - Simulated the agent's action by:
     - Determining the next state.
     - Calculating the reward.
     - Checking whether the episode is done (Goal or Hole reached).

4. **Implemented Scenarios**  
   - **Situation 1:** Took the agent to the Goal (G) in **2 steps**:
     - Actions: **Right → Right**.
   - **Situation 2:** Took the agent to the Hole (H) in **3 steps**:
     - Actions: **Down → Right → Right**.
   - **Situation 3:** Executed the trajectory **Down → Right → Up → Right**, calculated the cumulative reward, and compared it to Situation 1.  
     - Reward comparison indicates that Situation 1 is more optimal.
   - **Situation 4:** Designed a random-action agent that continues until it reaches the Goal (G). Displayed the number of episodes required to solve the task.

---



## **Outputs**
- **Situation 1:** Agent reached the Goal in **2 steps**.
- **Situation 2:** Agent reached the Hole in **3 steps**.
- **Situation 3:** Calculated cumulative reward and compared it with Situation 1.
- **Situation 4:** Agent used random actions to solve the task; number of episodes required is displayed.

---

## **Challenges and Insights**
- Designing the reward and transition tables required careful consideration of the environment's rules and terminal states.
- Comparing cumulative rewards highlighted the importance of optimizing trajectories in reinforcement learning.
- The random-action agent demonstrated how exploration is essential in solving reinforcement learning tasks.

---

**Note:** This notebook was submitted to **Wiem Khlifi** via email before the deadline.  

**Happy Learning!**

