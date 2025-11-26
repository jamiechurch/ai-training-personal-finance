# Personal Finance Analysis with Claude Code

**Analyze finances with AI in 15 minutes - no coding required**

Go from "never heard of this" to analyzing 75 financial documents with AI agents in three simple steps.

---

## 🚀 3-Step Quick Start

### Step 1: Install Claude Code
**Mac:** `brew install claude-code` or download from https://claude.ai/code
**Windows:** Download from https://claude.ai/code

### Step 2: Clone & Open
**Mac:**
```bash
git clone https://github.com/YOUR-USERNAME/AI-Training-Personal-Finance.git
cd AI\ Training\ Personal\ Finance
claude
```

**Windows:**
```powershell
git clone https://github.com/YOUR-USERNAME/AI-Training-Personal-Finance.git
cd "AI Training Personal Finance"
claude
```

**Optional:** Want sample data to practice with? See [DATA.md](DATA.md) for download instructions.

### Step 3: Run Your First Analysis
```
@spending-analyzer analyze January 2024 spending
```

✅ **Success!** You just analyzed a month of financial data in seconds.

---

## 💡 What You'll Learn

This project includes **4 powerful AI agents** that analyze personal finance data:

1. **Spending Analyzer** - Breaks down spending by category
2. **Cash Flow Analyst** - Tracks money in vs. money out
3. **Budget Monitor** - Evaluates against the 50/30/20 rule
4. **Retirement Analyzer** - Analyzes 401(k)/403(b) performance

Each agent reads real financial documents (75 PDFs) and provides instant insights that would take hours manually.

→ **[Try the full tutorial](TUTORIAL.md)** to learn all four agents

---

## 🎯 Example Output

```
$ @spending-analyzer analyze Q1 2024 spending

Q1 2024 Spending Analysis:

Housing:         $6,645.81  (mortgage)
Transportation:  $2,667.00  (vehicles, insurance, gas)
Gambling:        $2,100.00  (Jane's DraftKings - 13% of income!)
Groceries:       $2,145.00
Utilities:       $895.00
Dining Out:      $956.00

Total Spending:  $17,868.81
Total Income:    $29,014.92
Savings Rate:    38.4% ✓

Notable Patterns:
- Gambling expenses concerning at 13.1% of net income
- Excellent savings rate—maintain or increase
- Grocery spending is consistent month-over-month
```

---

## 📚 Next Steps

### For Learners
1. ✅ Complete the Quick Start above
2. 📖 **[Work through TUTORIAL.md](TUTORIAL.md)** - 15-minute main exercise
3. 🔍 **[Explore QUICK_REFERENCE.md](docs/QUICK_REFERENCE.md)** - All agents at a glance

### For Teachers
1. 📖 Review [TUTORIAL.md](TUTORIAL.md) completely
2. 💬 Use Part 4 "Teaching This to Others" for workshop planning
3. 🎤 2-hour workshop outline included

### For Advanced Users
1. 🔧 Study agent definitions in `.claude/agents/`
2. ✏️ Create your own custom agents
3. 🔄 Apply to your own data/domain

---

## 🛠️ Common Issues

### "Command not found: claude"
- Verify installation: `claude --version`
- Close and reopen your terminal
- Windows: Try running PowerShell as Administrator

### "Agent not found"
- Verify you're in the project directory: `pwd` (Mac) or `cd` (Windows)
- Check agents exist: `ls .claude/agents/`
- Make sure you typed `@agent-name` with the `@` symbol

### "Cannot read PDF files"
- You need financial documents to analyze
- Use your own PDFs in the `data/` folder, OR
- Download sample data - see [DATA.md](DATA.md) for instructions

→ **More help?** See [TUTORIAL.md - Advanced Topics](TUTORIAL.md#part-5-advanced-topics)

---

## 📦 Using Your Own Data or Sample Data

**Want to try it with your own financial documents?**
- Add your PDFs to the `data/` folder and start analyzing immediately

**Want to practice with sample data first?**
- See [DATA.md](DATA.md) for optional download of "Bob & Jane Doe" sample dataset
- 75 realistic financial documents (statements, tax returns, utility bills)
- Entirely fictional and generated for educational purposes

The agents work with any financial documents - use whatever fits your learning style.

---

## 🎓 What Makes This Special

- **Real-world ready**: Actually useful analysis, not toy examples
- **No programming**: Create powerful tools with plain English
- **Complete dataset**: 75 realistic documents to practice with
- **Teaching-focused**: Designed for workshops and demonstrations
- **4 ready-to-use agents**: Demonstrates variety of practical use cases

---

## 🤝 Contributing

This is a teaching/demonstration project. Feel free to:
- Create additional agents
- Improve existing agents
- Add more use case examples
- Share your workshop experiences

---

## 📞 Support & Resources

- **Getting Started**: [TUTORIAL.md](TUTORIAL.md)
- **Quick Reference**: [docs/QUICK_REFERENCE.md](docs/QUICK_REFERENCE.md)
- **Agent Definitions**: `.claude/agents/` directory
- **Claude Code Docs**: https://claude.ai/code/docs

---

**Ready to see AI-powered financial analysis in action?**

```bash
claude
@spending-analyzer analyze January 2024 spending
```

Let's get started! 🚀
