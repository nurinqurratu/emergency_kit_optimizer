# 🧰 Emergency Kit Optimizer (Dynamic Programming)  

The **Emergency Kit Optimizer** is a Python-based tool that helps travellers and outdoor enthusiasts pack essential survival items under **strict weight constraints**.  

By applying the **0/1 Knapsack dynamic programming algorithm**, the system ensures that the selected items maximize overall utility (survival value) without exceeding the allowable load.  

---

## 🌍 Real-Life Motivation  
Travellers often face challenges when packing:  
- A **hiker** may choose items manually and discover at the trailhead that the pack is too heavy or missing a flashlight.  
- A **family on a road trip** may overlook essentials like a stove or emergency blanket due to space limits.  

The Emergency Kit Optimizer solves these issues by:  
- Allowing users to input items with **weights and utility values**.  
- Producing an **optimal packing list** that balances necessity and weight.  
- Minimizing the risk of forgetting vital gear or carrying excess.  

---

## 🎯 Objectives  
1. Input a list of items with weights and survival utility values.  
2. Apply the **0/1 Knapsack dynamic programming algorithm** to maximize total utility.  
3. Generate an optimized packing list that fits within the user’s specified weight limit.  

---

## 🧑‍💻 Solution Approach  
- **Dynamic Programming (DP)**: Breaks down the problem into overlapping subproblems and stores results to avoid redundancy.  
- Builds a **2D DP table**:  
  - Rows → Items considered.  
  - Columns → Weight capacities up to the specified limit.  
- For each item:  
  - Exclude it (carry forward the best value so far).  
  - Or include it (add its utility + best value at reduced capacity).  
- After populating the table, **backtracking** determines which items were selected.  

✅ This ensures a **systematic and efficient solution** in polynomial time.  

---

## 📊 Example Use Case  
Input:  
- Weight limit = 15  
- Items =  
  - Water (weight 5, utility 10)  
  - First Aid Kit (weight 3, utility 7)  
  - Food Rations (weight 4, utility 9)  
  - Flashlight (weight 2, utility 5)  

Output:  
- Optimal selection = **Water + First Aid Kit + Flashlight**  
- Total weight = 10  
- Total utility = 22  

---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/nurinqurratu/emergency-kit-optimizer.git

