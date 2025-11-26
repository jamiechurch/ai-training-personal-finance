# Claude Code + Agents: Personal Finance Analysis Tutorial

**Get from zero to analyzing financial data in 15 minutes.**

---

## Part 1: 15-Minute Quick Start

### Install Claude Code (2 minutes)

**Mac:**
```bash
brew install claude-code
```
Or download from https://claude.ai/code

**Windows:**
Download and install from https://claude.ai/code

Verify: `claude --version`

### Clone the Project (1 minute)

**Mac:**
```bash
cd ~/Documents
git clone https://github.com/YOUR-USERNAME/AI-Training-Personal-Finance.git
cd AI\ Training\ Personal\ Finance
```

**Windows:**
```powershell
cd %USERPROFILE%\Documents
git clone https://github.com/YOUR-USERNAME/AI-Training-Personal-Finance.git
cd "AI Training Personal Finance"
```

### Run Your First Analysis (12 minutes)

Start Claude Code:
```bash
claude
```

**Try these commands in sequence:**

```
@spending-analyzer analyze Q1 2024 spending
```

```
@cashflow-analyst identify risky months
```

```
@budget-monitor evaluate against 50/30/20 rule
```

### What Just Happened?

You just used **3 AI agents** to analyze 75 financial documents in under a minute:

1. **Spending Analyzer** - Categorized every expense across 3 months
2. **Cash Flow Analyst** - Identified months with tight cash flow
3. **Budget Monitor** - Evaluated spending against financial best practices

Each agent read real PDFs, extracted data, performed calculations, and provided actionable insights. Manually, this would take hours.

### Try More

**Retirement analysis:**
```
@retirement-analyzer compare Bob and Jane's accounts
```

**Ask follow-up questions:**
```
What percentage of income goes to gambling?
```

```
Which month had the lowest balance?
```

**Explore other agents:** See [Part 2: Understanding Agents](#part-2-understanding-agents) below.

---

## Part 2: Understanding Agents

### What is an Agent?

An agent is a specialized AI assistant with:
- **Specific expertise** (e.g., cash flow analysis)
- **Clear objectives** (e.g., identify low balance months)
- **Consistent behavior** across uses

### The 4 Core Agents

#### 1. Spending Analyzer
**What it does:** Breaks down spending by category

**Use it for:**
- Monthly spending breakdowns
- Identifying spending trends
- Finding cost-cutting opportunities

**Example:** `@spending-analyzer analyze January 2024`

#### 2. Cash Flow Analyst
**What it does:** Tracks money in vs. money out

**Use it for:**
- Identifying tight cash flow months
- Analyzing payday timing impacts
- Preventing overdrafts

**Example:** `@cashflow-analyst review March 2024`

#### 3. Budget Monitor
**What it does:** Evaluates spending against the 50/30/20 rule

**Use it for:**
- Assessing overall financial health
- Identifying overspending categories
- Getting budget recommendations

**Example:** `@budget-monitor evaluate budget health`

#### 4. Retirement Analyzer
**What it does:** Analyzes 401(k) and 403(b) performance

**Use it for:**
- Calculating investment returns
- Comparing account performance
- Projecting retirement readiness

**Example:** `@retirement-analyzer compare retirement accounts`

### Additional Agents

Three more specialized agents are available for advanced use:
- **Tax Verifier** - Verifies tax return accuracy
- **Document Checker** - Confirms all files are present
- **Financial Auditor** - Cross-checks transaction accuracy

Explore these after mastering the core 4 agents.

---

## Part 3: The Main Exercise

### Complete Financial Health Check (10 minutes)

🎯 **Objective:** Get a complete picture of Bob & Jane's financial health

This exercise uses 3 agents in sequence to demonstrate how they work together.

#### Step 1: Analyze Spending Patterns

**Command:**
```
@spending-analyzer analyze Q1 2024 spending
```

**Expected output:**
```
Q1 2024 Spending Summary:

Housing:         $6,645.81  (27% of net income)
Transportation:  $2,667.00  (11% of net income)
Gambling:        $2,100.00  (13% of net income - concerning!)
Groceries:       $2,145.00  (8% of net income)
Utilities:       $895.00    (4% of net income)
Dining Out:      $956.00    (6% of net income)

Total Spending:  $17,868.81
Total Income:    $29,014.92
Savings Rate:    38.4% ✓
```

💡 **Learning Points:**
- Agent categorizes expenses automatically
- Calculates percentages and identifies concerns
- Shows savings rate (38.4% is excellent!)

#### Step 2: Check Cash Flow Health

**Command:**
```
@cashflow-analyst identify risky months
```

**Expected output:**
```
Cash Flow Analysis:

Minimum Balance by Month:
- January: $3,247 (after mortgage payment)
- February: $2,891 (lowest - mid-month before payday)
- March: $3,105 (after large tax payment)

Pattern Identified:
- Balances lowest around the 14th (between paychecks)
- Bob & Jane are paid bi-monthly (1st and 15th)
- Tight window between expenses and income

Recommendation:
Build a $2,000 cash buffer to avoid tight timing issues.
```

💡 **Learning Points:**
- Agent identifies timing issues automatically
- Recognizes paycheck patterns
- Provides actionable recommendations

#### Step 3: Evaluate Budget Compliance

**Command:**
```
@budget-monitor evaluate against 50/30/20 rule
```

**Expected output:**
```
50/30/20 Rule Analysis:

Needs (target 50%): 62% ❌ OVER BUDGET
  Housing:         27%
  Transportation:  11%
  Insurance:       9%
  Utilities:       4%
  Groceries:       8%
  Other:           3%

Wants (target 30%): 28% ✅ ON TARGET
  Dining:          6%
  Gambling:        9%
  Entertainment:   5%
  Shopping:        8%

Savings (target 20%): 10% ❌ UNDER TARGET

Key Issues:
1. "Needs" over budget due to high housing + transportation costs
2. Savings below 20% target despite 38% savings rate (calculation difference)
3. Gambling expenses (9% of budget) are concerning

Recommendations:
- Consider refinancing mortgage or downsizing vehicle
- Address gambling expenses
- Increase automatic savings contributions
```

💡 **Learning Points:**
- Agent applies financial frameworks automatically
- Visual indicators (✅/❌) make issues clear
- Prioritizes action items

#### Wrap-Up: What You Discovered

In 10 minutes, you:

1. ✅ Identified Bob & Jane have excellent savings (38.4% rate)
2. ⚠️ Found concerning gambling expenses ($700/month)
3. ⚠️ Discovered tight cash flow mid-month
4. ⚠️ Identified "needs" are over the 50% budget target
5. 💡 Got actionable recommendations (build buffer, address gambling)

**This analysis would take hours manually. With agents: under 1 minute.**

### Optional: Try Other Agents

**Retirement Analysis:**
```
@retirement-analyzer compare Bob and Jane's retirement accounts
```

**Tax Verification:**
```
@tax-verifier verify 2023 Form 1040
```

**Ask follow-up questions:**
```
At this savings rate, when could they retire early?
```

```
What if they eliminated gambling expenses?
```

---

## Part 4: Teaching This to Others

### 2-Hour Workshop Outline

**Part 1: Introduction (15 min)**
- What are AI agents?
- Why use them for financial analysis?
- Quick demo of one agent

**Part 2: Live Demo (30 min)**
- Show spending-analyzer with real output
- Show cashflow-analyst identifying problems
- Demonstrate follow-up questions
- Key message: "Hours of work in seconds"

**Part 3: Hands-On Practice (60 min)**
- Participants run the main exercise (Part 3)
- Guide through all 3 steps
- Help with questions and troubleshooting
- Encourage experimentation

**Part 4: Discussion & Next Steps (15 min)**
- What other use cases can you imagine?
- How could this apply to your work?
- How to create custom agents
- Q&A

### Key Talking Points

🎯 **Speed:** "What takes hours manually takes seconds with agents"

🎯 **Accuracy:** "Agents don't make arithmetic errors or miss transactions"

🎯 **Consistency:** "Same rigorous analysis every time - no shortcuts"

🎯 **Scalability:** "Analyze 10 files or 10,000 files with the same effort"

🎯 **Accessibility:** "No programming required - just clear English instructions"

### Common Workshop Questions

**Q: Can agents make mistakes?**
A: Yes. Always verify critical calculations. Agents assist human judgment, not replace it.

**Q: Do I need programming skills?**
A: No! Agents are defined in markdown files with plain English.

**Q: Can I use my own data?**
A: Absolutely. Replace sample PDFs with your own financial documents.

**Q: How much does Claude Code cost?**
A: See pricing at claude.ai/code. Consider cost vs. hours saved.

**Q: What other domains can use agents?**
A: Legal document analysis, healthcare records, business operations, research - any document-heavy domain.

---

## Part 5: Advanced Topics

### Creating Custom Agents

**Basic Template:**
```markdown
You are a [specialist role]. Analyze Bob and Jane's financial documents and:

1. [Specific task 1]
2. [Specific task 2]
3. [Specific task 3]

Context:
- [Relevant background information]
- [Key constraints or considerations]

Output format:
- [How to present results]
- [What to highlight]
```

**Example: Debt Reduction Planner**

File: `.claude/agents/debt-planner.md`

```markdown
You are a debt reduction specialist. Analyze Bob and Jane's financial
documents and create a personalized debt payoff plan:

1. Identify all debt obligations (mortgage, vehicle loans)
2. Calculate total monthly debt payments
3. Determine debt-to-income ratio
4. Analyze available extra cash for debt paydown
5. Create a debt snowball or avalanche strategy
6. Project debt-free timeline under different scenarios

Financial Context:
- Mortgage: $2,215/month
- Ford F-150: $504/month
- Harley Davidson: $385/month
- Combined income: $160,000/year
- Current savings rate: 38%

Provide actionable plan with timelines and projected interest savings.
```

**Usage:** `@debt-planner create payoff strategy`

### Agent Design Best Practices

1. **Single Responsibility** - One clear purpose per agent
2. **Specific Instructions** - Tell the agent exactly what to analyze
3. **Provide Context** - Include relevant background information
4. **Define Output Format** - Specify how to present results
5. **Include Examples** - Show expected output when helpful

### Advanced Workflows

**Monthly Financial Review:**
```
@spending-analyzer breakdown [month] spending
@cashflow-analyst review [month] cash flow
@budget-monitor evaluate [month] compliance
```

**Annual Summary:**
```
@spending-analyzer analyze full year trends
@retirement-analyzer review account performance
@tax-verifier prepare for tax season
```

**Problem Investigation:**
```
@cashflow-analyst why was March balance so low?
@spending-analyzer show March anomalies
[Follow-up questions to drill down]
```

### Expanding to Other Domains

**Legal Document Analysis:**
- Contract reviewer agent
- Compliance checker agent
- Risk assessment agent

**Healthcare Records:**
- Medical history analyzer
- Medication interaction checker
- Test results tracker

**Business Operations:**
- Sales pipeline analyzer
- Customer churn predictor
- Inventory optimizer

**Academic Research:**
- Literature review agent
- Data quality checker
- Citation verifier

---

## Appendix: Detailed Setup Guide

### Complete Beginner Setup

If you've never used a command line before, this section walks through everything step-by-step.

#### What is a Terminal/Command Line?

The command line is a way to talk directly to your computer using text commands instead of clicking buttons.

**Mac users:** It's called "Terminal"
**Windows users:** It's called "Command Prompt" or "PowerShell"

#### Opening Your Terminal

**On Mac:**
1. Press **Command + Space**
2. Type "Terminal"
3. Press Enter

**On Windows:**
1. Press **Windows key**
2. Type "PowerShell"
3. Press Enter

#### Basic Commands You Need

**Navigate to a folder:**
```bash
cd Documents
```

**See where you are:**
- Mac: `pwd`
- Windows: `cd`

**List files in current location:**
- Mac: `ls`
- Windows: `dir`

**Go up one folder level:**
```bash
cd ..
```

#### Step-by-Step Installation

**1. Install Git (for downloading projects)**

Mac: Download from https://git-scm.com/download/mac
Windows: Download from https://git-scm.com/download/windows

Verify: `git --version`

**2. Install Claude Code**

Mac: `brew install claude-code` or download from https://claude.ai/code
Windows: Download from https://claude.ai/code

Verify: `claude --version`

**3. Download This Project**

Navigate to Documents:
```bash
# Mac
cd ~/Documents

# Windows
cd %USERPROFILE%\Documents
```

Clone the project:
```bash
git clone https://github.com/YOUR-USERNAME/AI-Training-Personal-Finance.git
```

Enter the project folder:
```bash
# Mac
cd AI\ Training\ Personal\ Finance

# Windows
cd "AI Training Personal Finance"
```

**4. Verify Setup**

Check you're in the right place:
```bash
# Mac
pwd

# Windows
cd
```

Should show path ending in "AI Training Personal Finance"

List files:
```bash
# Mac
ls

# Windows
dir
```

Should see: `.claude`, `data`, `README.md`, `TUTORIAL.md`

Check agents exist:
```bash
ls .claude/agents
```

Should see 8 `.md` files (the agents)

**5. Start Analyzing**

Launch Claude Code:
```bash
claude
```

Run your first agent:
```
@spending-analyzer analyze January 2024
```

✅ Success! You're analyzing financial data with AI.

#### Common Setup Problems

**"Command not found: claude"**
- Close and reopen your terminal
- Verify installation with `claude --version`
- Windows: Try running PowerShell as Administrator

**"Agent not found"**
- Verify you're in the project directory: `pwd` or `cd`
- Check agents exist: `ls .claude/agents/`
- Make sure you used the `@` symbol

**"No such file or directory"**
- Navigate back to project: `cd ~/Documents/AI\ Training\ Personal\ Finance` (Mac)
- Or: `cd %USERPROFILE%\Documents\"AI Training Personal Finance"` (Windows)

**"Cannot read PDF files"**
- Verify files exist: `ls data/bobandjanedoe/statements/checking/`
- Should show 12 PDF files
- If missing: Re-clone the repository

**"Permission denied"**
- Mac: Grant Terminal permissions in System Preferences > Security & Privacy
- Windows: Run PowerShell as Administrator (right-click > Run as Administrator)

---

## Resources

**Documentation:**
- Claude Code Docs: https://claude.ai/code/docs
- Agent Definitions: `.claude/agents/` directory
- Sample Data: `data/bobandjanedoe/` directory

**Project Files:**
- Agent definitions: `.claude/agents/*.md`
- Financial data: `data/bobandjanedoe/statements/`
- Data generators: `data/bobandjanedoe/generate_*.py`

**Next Steps:**
1. Complete the main exercise (Part 3)
2. Try all 4 core agents
3. Create your own custom agent
4. Apply to your own data
5. Teach others what you learned

---

## About the Sample Data

**Bob & Jane Doe** (fictional couple)
- Bob: 47, Security Guard, $95K/year
- Jane: 45, Teacher, $65K/year
- Location: Nashville, TN
- Combined Income: $160K/year

**75 Realistic Financial Documents:**
- 12 checking statements (all of 2024)
- 12 savings statements (all of 2024)
- 2 retirement accounts (Bob's 401k, Jane's 403b)
- 1 tax return (2023 Form 1040)
- 48 utility bills (4 utilities × 12 months)

All data is entirely fictional and generated for educational purposes.

---

**Questions or feedback?** Review agent files in `.claude/agents/`, experiment with different prompts, and create your own custom agents!

**Ready to start?** Jump to [Part 1: 15-Minute Quick Start](#part-1-15-minute-quick-start)

Welcome to AI-assisted financial analysis! 🚀
