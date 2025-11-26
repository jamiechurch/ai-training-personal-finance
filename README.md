# Personal Finance Analysis with Claude Code + Agents

## 🎯 Purpose

This project demonstrates the power of Claude Code and AI agents for financial analysis. It's designed as a **teaching tool** to show others how to leverage AI for practical, real-world tasks without writing code.

## ✨ What This Project Does

Analyzes a complete set of fictional financial documents (75 PDFs) using 8 specialized AI agents:

1. **Document Completeness Checker** - Verifies all files are present
2. **Financial Auditor** - Cross-references transactions and verifies accuracy
3. **Spending Pattern Analyzer** - Breaks down spending by category
4. **Cash Flow Analyst** - Tracks money in vs. money out
5. **Budget Compliance Monitor** - Evaluates against budgeting best practices
6. **Savings Goal Tracker** - Monitors savings progress and growth
7. **Retirement Account Analyzer** - Evaluates 401(k) and 403(b) performance
8. **Tax Document Verifier** - Verifies tax return accuracy

## 🚀 Quick Start

### Prerequisites

- [Claude Code](https://claude.ai/code) installed
- This repository cloned to your machine

### 5-Minute Demo

1. **Open Claude Code** in this directory

2. **Verify the setup**:
   ```
   @document-checker verify all files are present
   ```

3. **Run your first analysis**:
   ```
   @spending-analyzer analyze January 2024 spending
   ```

4. **See the power**:
   ```
   @budget-monitor evaluate budget health
   ```

That's it! You just performed financial analysis that would typically take hours.

## 📚 Project Structure

```
├── .claude/
│   └── agents/              # 8 custom AI agents
├── data/
│   └── bobandjanedoe/       # 75 financial PDFs + generators
│       └── statements/
│           ├── checking/    # 12 monthly statements
│           ├── savings/     # 12 monthly statements
│           ├── retirement/  # 2 annual statements
│           ├── tax/         # 1 tax return
│           └── utilities/   # 48 utility bills
├── docs/                    # Additional documentation
├── examples/                # Example analysis outputs
├── TUTORIAL.md             # Comprehensive tutorial (start here!)
└── README.md               # This file
```

## 🎓 Learning Path

### For Beginners
1. Read this README
2. Try the Quick Start above
3. Work through [TUTORIAL.md](TUTORIAL.md) exercises 1-4

### For Trainers
1. Review [TUTORIAL.md](TUTORIAL.md) completely
2. Practice the 8 exercises
3. Use Part 6 "Teaching This to Others" for workshop planning

### For Advanced Users
1. Study the agent definitions in `.claude/agents/`
2. Create your own custom agents
3. Apply to your own data/domain

## 💡 Key Concepts

### What is Claude Code?

Claude Code is an AI-powered CLI tool that helps with various tasks including code, analysis, and automation.

### What are Agents?

Agents are specialized AI assistants with:
- **Specific expertise** (e.g., tax verification)
- **Clear objectives** (e.g., verify calculations)
- **Consistent behavior** across uses

### Why Use Agents for Finance?

- **Speed**: Analyze months of data in seconds
- **Accuracy**: No arithmetic errors, catches inconsistencies
- **Insights**: Identifies patterns humans might miss
- **Accessibility**: No programming knowledge required

## 🏗️ The Sample Data

### Bob and Jane Doe (Fictional Couple)

- **Bob**: 47, Security Guard, $95K/year
- **Jane**: 45, Teacher, $65K/year
- **Location**: Nashville, TN
- **Combined Income**: $160K/year

### Financial Documents (All Fictional)

- 12 months of checking statements (2024)
- 12 months of savings statements (2024)
- 2 retirement account statements (401k, 403b)
- 1 tax return (2023 Form 1040)
- 48 utility bills (electric, gas, water, internet)

**Total: 75 PDF files** with realistic transaction patterns

## 🎯 Example Use Cases

### Use Case 1: Monthly Financial Review
```
@financial-auditor audit January 2024
@spending-analyzer show January spending breakdown
@cashflow-analyst review January cash flow
```

### Use Case 2: Annual Summary
```
@spending-analyzer analyze full year trends
@savings-tracker calculate 2024 progress
@retirement-analyzer compare account performance
```

### Use Case 3: Budget Planning
```
@budget-monitor evaluate against 50/30/20 rule
@cashflow-analyst identify available cash
@spending-analyzer find cost-cutting opportunities
```

### Use Case 4: Tax Preparation
```
@tax-verifier verify 2023 Form 1040
@savings-tracker calculate interest income
@retirement-analyzer summarize contributions
```

## 🔧 Customization

### Create Your Own Agent

1. Create a new file in `.claude/agents/your-agent-name.md`
2. Write clear instructions for what the agent should do
3. Invoke with `@your-agent-name [your question]`

**Example**: Gambling Expense Analyzer
```markdown
You are a financial counselor. Analyze Jane's DraftKings gambling
expenses across all 2024 checking statements and:

1. Calculate total spent per month
2. Identify patterns (day of week, time of month)
3. Calculate as percentage of income
4. Provide recommendations for management
```

### Use Your Own Data

Replace the sample PDFs in `data/bobandjanedoe/statements/` with your own financial documents, then run the same agents!

## 📖 Full Tutorial

For a comprehensive, step-by-step guide with 8 hands-on exercises, see **[TUTORIAL.md](TUTORIAL.md)**

Topics covered:
- Understanding agents in depth
- 8 complete exercises with expected outputs
- Advanced workflows
- Creating custom agents
- Teaching workshops (2-hour outline)
- Expanding to other domains

## 🎤 Teaching This to Others

### Workshop Format (2 hours)

1. **Introduction** (15 min): What are agents? Why use them?
2. **Live Demo** (30 min): Show the power with 2-3 agents
3. **Hands-On** (60 min): Participants run exercises
4. **Discussion** (15 min): Applications, Q&A

### Key Talking Points

- "What takes hours manually takes seconds with agents"
- "No programming required—just clear English instructions"
- "Same analysis approach every time—consistent and reliable"
- "Scales from 10 files to 10,000 files with same effort"

## 🌟 What Makes This Special

1. **Real-world application**: Not a toy example, actually useful
2. **Complete data set**: 75 realistic financial documents
3. **8 ready-to-use agents**: Demonstrates variety of use cases
4. **No programming**: Accessible to non-technical users
5. **Teaching-focused**: Designed for workshops and demonstrations

## 🔍 Sample Output

```
$ @spending-analyzer analyze Q1 2024 spending

Q1 2024 Spending Analysis:

Housing: $6,645.81 (mortgage)
Transportation: $2,667 (vehicles, insurance, gas)
Gambling: $2,100 (Jane's DraftKings)
Groceries: $2,145
Utilities: $895
Dining Out: $956
Insurance: $1,350 (health, life)
Entertainment: $487
Shopping: $623

Total Spending: $17,868.81
Total Income: $29,014.92
Savings Rate: 38.4%

Notable Patterns:
- Gambling expenses are concerning at 13.1% of net income
- Grocery spending is consistent month-over-month
- Dining out decreased in March (tax season awareness?)

Recommendations:
- Address gambling expenses (consider setting stricter limits)
- Excellent savings rate—maintain or increase
- Consider meal planning to reduce grocery costs further
```

## 🛠️ Troubleshooting

### "Agent not found"
- Ensure you're in the project directory
- Verify `.claude/agents/[agent-name].md` exists
- Try `ls .claude/agents/` to see available agents

### "Cannot read PDF files"
- Verify PDFs exist: `find data/bobandjanedoe/statements -name "*.pdf" | wc -l` (should show 75)
- Try opening a PDF manually to ensure they're not corrupted
- Regenerate if needed using Python scripts in `data/bobandjanedoe/`

### "Agent gives generic responses"
- Be more specific in your questions
- Reference specific months or documents
- Ask for numerical analysis rather than general observations

## 📦 Dependencies

For using the project:
- Claude Code (no other dependencies!)

For regenerating financial PDFs (optional):
- Python 3.8+
- fpdf2 (`pip install -r data/bobandjanedoe/requirements.txt`)

## 🤝 Contributing

This is a teaching/demonstration project. Feel free to:
- Create additional agents
- Improve existing agents
- Add more use case examples
- Share your workshop experiences

## 📄 License

The financial data is entirely fictional and generated for educational purposes. All sample documents include disclaimers.

## 🙏 Acknowledgments

- Financial data generator: See `data/bobandjanedoe/README.md`
- Inspired by real personal finance challenges
- Built to demonstrate Claude Code's agent capabilities

## 📞 Support

- **Start here**: [TUTORIAL.md](TUTORIAL.md)
- **Agent reference**: See files in `.claude/agents/`
- **Data documentation**: `data/bobandjanedoe/README.md`
- **Claude Code docs**: [claude.ai/code/docs](https://claude.ai/code/docs)

## 🎯 Next Steps

1. **Try it now**: Run the Quick Start above
2. **Learn more**: Read [TUTORIAL.md](TUTORIAL.md)
3. **Experiment**: Ask agents different questions
4. **Create**: Build your own custom agent
5. **Share**: Teach others what you've learned

---

**Ready to see AI-powered financial analysis in action?**

```
@document-checker verify all files are present
```

Let's get started! 🚀
