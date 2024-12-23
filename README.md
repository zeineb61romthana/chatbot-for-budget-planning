# 📊 Finance Chatbot: Budget Planner 🤖

Welcome to the **Finance Chatbot** project! This chatbot helps users organize their budget using the **50/30/20 rule** and provides personalized savings tips based on their income and expenses.

## 🛠️ How to Run the Chatbot

### Step 1: Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/zeineb61romthana/chatbot-for-budget-planning.git
   
Install the required dependencies:

````bash
pip install -r requirements.txt



Set up the Gemini API key :

````bash
export GOOGLE_API_KEY='api_key'

### Step 2: run the chatbot
To run the chatbot, simply execute the Python notebook.

## 💡 **Explanation of How the Budget is Calculated and How Savings Tips are Generated**

### 📏 **Budget Calculation (50/30/20 Rule)**

The **50/30/20 rule** divides your monthly income into three categories:

1. **Needs (50%)**: Essential expenses like housing, utilities, and groceries.
2. **Wants (30%)**: Non-essential expenses such as entertainment, dining, and hobbies.
3. **Savings (20%)**: Money saved or invested for future goals.

#### Example Calculation:

If your monthly income is **$5000**, here's how the budget is calculated:

- **Needs** = $5000 * 0.5 = **$2500**
- **Wants** = $5000 * 0.3 = **$1500**
- **Savings** = $5000 * 0.2 = **$1000**

These values are calculated using the `BudgetCalculatorTool`.

### 💸 **Savings Tips Generation**

The **ExpenseAnalyzerTool** generates savings tips by comparing your actual spending in the "needs" and "wants" categories with the recommended percentages from the 50/30/20 rule:

- If **actual needs** exceed 50% of income, the tool suggests reducing fixed costs.
- If **actual wants** exceed 30%, the tool recommends cutting back on discretionary spending.

#### Example:

If your actual **needs** are **$3000** (higher than the recommended 50%) and your **wants** are **$1800** (higher than the recommended 30%), the tool will suggest:

- **Reduce fixed costs** in essential expenses.
- **Cut back on discretionary spending** by a specific amount.

These tips are returned by the `ExpenseAnalyzerTool` as actionable recommendations.
