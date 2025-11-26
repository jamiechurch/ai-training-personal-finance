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

Note: If you're new to command line tools, see the **First Time Setup** section below before starting the 5-Minute Demo.

### First Time Setup

If this is your first time using Claude Code or working with command line tools, follow these steps:

#### 1. Install Required Software

**Claude Code:**
- Mac: Download from https://claude.ai/code and follow installer
- Windows: Download from https://claude.ai/code and run installer

**Git (for downloading this project):**
- Mac: Download from https://git-scm.com/download/mac
- Windows: Download from https://git-scm.com/download/windows

Tip: After installation, close and reopen your Terminal (Mac) or Command Prompt/PowerShell (Windows).

#### 2. Open Your Command Line

**Mac Users:**
- Open **Terminal**: Go to Applications > Utilities > Terminal
- Or press **Command + Space**, type "Terminal", press Enter

**Windows Users:**
- Open **PowerShell**: Click Start, type "PowerShell", press Enter
- Or right-click Start and select "Windows PowerShell"

#### 3. Download This Project

Navigate to where you want to store the project (we recommend Documents):

**Mac:**
```bash
cd ~/Documents
git clone https://github.com/YOUR-GITHUB-USERNAME/AI-Training-Personal-Finance.git
cd AI\ Training\ Personal\ Finance
```

**Windows:**
```powershell
cd %USERPROFILE%\Documents
git clone https://github.com/YOUR-GITHUB-USERNAME/AI-Training-Personal-Finance.git
cd "AI Training Personal Finance"
```

Note: Replace `YOUR-GITHUB-USERNAME` with the actual GitHub username where this project is stored. If you don't have a GitHub URL, download the project as a ZIP file and extract it to your Documents folder.

#### 4. Verify Everything Works

Check that files downloaded correctly:

**Mac:**
```bash
ls
```

**Windows:**
```powershell
dir
```

Success: You should see folders including `.claude`, `data`, and files like `README.md` and `TUTORIAL.md`.

Check that agents are present:

**Mac/Windows:**
```bash
ls .claude/agents
```

Success: You should see files like `spending-analyzer.md`, `cashflow-analyst.md`, etc.

Tip: For detailed beginner-friendly instructions with screenshots and troubleshooting, see the **"Setup Instructions for Beginners"** section in [TUTORIAL.md](TUTORIAL.md).

### 5-Minute Demo

Once you've completed the First Time Setup above, try this quick demonstration:

1. **Make sure you're in the project directory**

   **Mac:**
   ```bash
   pwd
   ```
   Should show: `/Users/YourName/Documents/AI Training Personal Finance`

   **Windows:**
   ```powershell
   cd
   ```
   Should show: `C:\Users\YourName\Documents\AI Training Personal Finance`

   Note: If you're not in the right location, navigate back using the commands in Step 3 of First Time Setup.

2. **Start Claude Code** in this directory:

   ```bash
   claude
   ```

   Success: You'll see a welcome message and a prompt (>).

3. **Verify the setup** by checking all files are present:
   ```
   @document-checker verify all files are present
   ```

   Success: The agent will confirm all 75 financial documents are present.

4. **Run your first analysis** - analyze January spending patterns:
   ```
   @spending-analyzer analyze January 2024 spending
   ```

   Success: You'll see a detailed breakdown of all spending by category!

5. **See the power** - evaluate overall budget health:
   ```
   @budget-monitor evaluate budget health
   ```

   Success: The agent will analyze spending against the 50/30/20 budgeting rule.

That's it! You just performed financial analysis that would typically take hours.

Tip: You can ask follow-up questions like "What percentage of income goes to gambling?" or "Which month had the highest spending?"

Note: For complete beginner instructions including how to open Terminal/PowerShell, navigate folders, and detailed troubleshooting, see [TUTORIAL.md](TUTORIAL.md) - "Setup Instructions for Beginners".

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

### "Command not found: claude"

**Mac Users:**
- Verify Claude Code is installed: Open Terminal and type `claude --version`
- If not installed, download from https://claude.ai/code
- After installing, close and reopen Terminal
- Try running the command again

**Windows Users:**
- Verify Claude Code is installed: Open PowerShell and type `claude --version`
- If not installed, download from https://claude.ai/code
- After installing, close and reopen PowerShell
- If still not working, try running PowerShell as Administrator (right-click > "Run as Administrator")

### "Agent not found"

**Solution:**
- Make sure you're in the correct project directory
  - Mac: Type `pwd` to check your location
  - Windows: Type `cd` to check your location
- Verify the agents folder exists: `ls .claude/agents/`
- Check you typed the agent name correctly (case-sensitive!)
- Make sure you're using the `@` symbol before the agent name

Note: Agent names use hyphens, not spaces: `@spending-analyzer` not `@spending analyzer`

### "Cannot read PDF files"

**Mac Users:**
```bash
ls data/bobandjanedoe/statements/checking/ | wc -l
```
Should show 12 files (12 monthly statements).

**Windows Users:**
```powershell
dir data\bobandjanedoe\statements\checking\
```
Should show 12 PDF files.

**If files are missing:**
- The download may have been incomplete
- Try cloning the repository again
- Check that Git downloaded all files (large repos sometimes have issues)
- Try opening a PDF manually to ensure they're not corrupted

### "Permission denied" or "Access denied"

**Mac Users:**
- You may need to grant Terminal permission to access files
- Go to **System Preferences > Security & Privacy > Privacy > Files and Folders**
- Ensure Terminal has necessary permissions
- Try using `sudo` before the command (will prompt for your password)

**Windows Users:**
- You may need to run PowerShell as Administrator
- Right-click on PowerShell and select **"Run as Administrator"**
- Navigate back to the project folder and try again
- Check that the files aren't marked as "Read Only"

### "Agent gives generic responses"

**Solution:**
- Be more specific in your questions
- Reference specific months or documents: "analyze January 2024" not just "analyze"
- Ask for numerical analysis: "calculate total gambling expenses" not "tell me about gambling"
- Ask follow-up questions to dig deeper
- Make sure you're asking the right agent for the task

Tip: Different agents have different specialties. Use `@spending-analyzer` for spending questions, `@cashflow-analyst` for balance questions, etc.

### Wrong directory / "No such file or directory"

**Mac Users:**
```bash
# Check where you are
pwd

# Navigate to your home directory
cd ~

# Navigate to Documents
cd Documents

# Navigate to project (use backslashes before spaces)
cd AI\ Training\ Personal\ Finance

# Verify you're in the right place
pwd
ls
```

**Windows Users:**
```powershell
# Check where you are
cd

# Navigate to Documents
cd %USERPROFILE%\Documents

# Navigate to project (use quotes around names with spaces)
cd "AI Training Personal Finance"

# Verify you're in the right place
cd
dir
```

Success: You should see `.claude`, `data`, `README.md`, and `TUTORIAL.md` when you list files.

### Still stuck?

Note: For complete beginner-friendly troubleshooting with detailed explanations, see the **"Setup Instructions for Beginners"** section in [TUTORIAL.md](TUTORIAL.md).

When asking for help, include:
- Your operating system (Mac or Windows)
- The exact command you typed
- The exact error message you received
- What directory you're in (output of `pwd` on Mac or `cd` on Windows)

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
