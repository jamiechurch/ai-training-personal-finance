# Claude Code + Agents: Personal Finance Analysis Tutorial

## Overview

This tutorial demonstrates the power of Claude Code with custom agents for financial analysis. You'll learn how to create specialized AI agents that analyze financial data, providing insights that would typically require hours of manual work.

## What You'll Learn

1. How to set up custom agents in Claude Code
2. How to use agents to analyze real financial data
3. Best practices for agent-based workflows
4. Practical applications of AI in personal finance

## Project Structure

```
AI Training Personal Finance/
├── .claude/
│   └── agents/              # Custom agent definitions (8 specialized agents)
│       ├── financial-auditor.md
│       ├── spending-analyzer.md
│       ├── tax-verifier.md
│       ├── retirement-analyzer.md
│       ├── budget-monitor.md
│       ├── cashflow-analyst.md
│       ├── document-checker.md
│       └── savings-tracker.md
├── data/
│   └── bobandjanedoe/       # Sample financial data (75 PDFs)
│       ├── statements/
│       │   ├── checking/    # 12 monthly bank statements
│       │   ├── savings/     # 12 monthly savings statements
│       │   ├── retirement/  # 2 annual retirement statements
│       │   ├── tax/         # 1 tax return (Form 1040)
│       │   └── utilities/   # 48 utility bills (4 types × 12 months)
│       └── generate_*.py    # Python scripts to regenerate data
├── docs/                    # Additional documentation
├── examples/                # Example analysis outputs
└── TUTORIAL.md             # This file
```

## The Story: Bob and Jane Doe

This project uses a complete set of fictional financial documents for a married couple:

- **Bob Doe** (47): Security Guard, $95,000/year
- **Jane Doe** (45): Elementary School Teacher, $65,000/year
- **Location**: Nashville, TN
- **Combined Income**: $160,000/year
- **Major Expenses**: Mortgage ($2,215/mo), vehicles, insurance, Jane's gambling habit ($700/mo)
- **Retirement Savings**: Bob's 401(k) ($169K), Jane's 403(b) ($116K)

## Prerequisites

- Claude Code installed and configured
- Basic understanding of personal finance concepts
- No programming knowledge required!

## Part 1: Understanding Agents in Claude Code

### What is an Agent?

An agent is a specialized AI assistant with:
- **Specific expertise** (e.g., financial auditing, tax preparation)
- **Clear objectives** (e.g., verify calculations, identify trends)
- **Consistent behavior** across multiple uses

### How Agents Work in Claude Code

1. **Agent Definition**: Stored in `.claude/agents/[agent-name].md`
2. **Invocation**: Use `@agent-name` in your conversation
3. **Execution**: Agent analyzes files and provides specialized insights
4. **Iteration**: Ask follow-up questions to dig deeper

### Benefits of Using Agents

- **Consistency**: Same analysis approach every time
- **Specialization**: Each agent focuses on specific tasks
- **Efficiency**: No need to re-explain context
- **Scalability**: Create once, use many times

## Part 2: The 8 Financial Analysis Agents

### Agent 1: Document Completeness Checker
**Purpose**: Verify all financial documents are present and accounted for

**Use Cases**:
- Before starting analysis, ensure no files are missing
- Audit file organization
- Verify data completeness after generating new documents

**Expected Output**: List of all files with confirmation of completeness

### Agent 2: Financial Auditor
**Purpose**: Cross-reference transactions and verify mathematical accuracy

**Use Cases**:
- Ensure utility bills match bank statement charges
- Verify running balances are calculated correctly
- Catch data generation errors
- Validate consistency across documents

**Expected Output**: Detailed audit report with any discrepancies highlighted

### Agent 3: Spending Pattern Analyzer
**Purpose**: Understand where money is being spent

**Use Cases**:
- Monthly spending breakdowns by category
- Identify spending trends over time
- Compare spending across months
- Find opportunities for cost savings

**Expected Output**: Comprehensive spending report with categorized expenses

### Agent 4: Cash Flow Analyst
**Purpose**: Track money in vs. money out

**Use Cases**:
- Identify months with tight cash flow
- Analyze impact of bi-monthly paychecks
- Predict potential overdraft situations
- Optimize payment timing

**Expected Output**: Month-by-month cash flow analysis with balance trends

### Agent 5: Budget Compliance Monitor
**Purpose**: Compare spending to budgeting best practices

**Use Cases**:
- Evaluate against 50/30/20 rule (needs/wants/savings)
- Identify overspending categories
- Assess financial health
- Generate actionable recommendations

**Expected Output**: Budget compliance report with recommendations

### Agent 6: Savings Goal Tracker
**Purpose**: Monitor savings progress and growth

**Use Cases**:
- Calculate total interest earned
- Verify monthly transfer goals are met
- Project future savings growth
- Assess savings rate vs. income

**Expected Output**: Savings progress report with future projections

### Agent 7: Retirement Account Analyzer
**Purpose**: Evaluate retirement savings performance

**Use Cases**:
- Calculate actual rate of return
- Compare 401(k) vs. 403(b) performance
- Analyze fund allocations
- Project retirement readiness

**Expected Output**: Comprehensive retirement analysis with projections

### Agent 8: Tax Document Verifier
**Purpose**: Verify tax return accuracy

**Use Cases**:
- Cross-check W-2 income
- Verify interest income from savings
- Validate tax calculations
- Ensure proper deductions

**Expected Output**: Tax verification report with any errors identified

## Part 3: Step-by-Step Tutorial

### Exercise 1: Document Verification

**Objective**: Verify all 75 financial documents are present

**Steps**:

1. Open Claude Code in this directory
2. Type: `@document-checker verify all files`
3. Review the output

**Expected Result**:
```
✓ 12 checking statements (Jan-Dec 2024)
✓ 12 savings statements (Jan-Dec 2024)
✓ 2 retirement statements (401k, 403b)
✓ 1 tax return (2023 Form 1040)
✓ 48 utility bills (electric, gas, water, internet)
Total: 75 files - All present and accounted for
```

**Learning Points**:
- Agents can quickly inventory large document sets
- Automated verification catches missing files
- Establishes baseline before deeper analysis

### Exercise 2: Financial Audit

**Objective**: Verify the accuracy of January 2024 statements

**Steps**:

1. Type: `@financial-auditor audit January 2024 statements`
2. Wait for the agent to analyze checking, savings, and utility bills
3. Review findings

**Expected Result**:
- Confirmation that utility bills match bank charges
- Verification of running balance calculations
- Cross-reference of savings transfer in both accounts
- Interest calculation verification

**Learning Points**:
- Agents can cross-reference multiple documents
- Catches mathematical errors humans might miss
- Essential for data quality assurance

### Exercise 3: Spending Analysis

**Objective**: Understand spending patterns for Q1 2024

**Steps**:

1. Type: `@spending-analyzer analyze Q1 2024 spending patterns`
2. Review the categorized breakdown
3. Ask follow-up: "Which category had the most variation?"
4. Ask: "What percentage of income goes to Jane's gambling?"

**Expected Result**:
```
Q1 2024 Spending Summary:
- Housing: $6,645 (mortgage)
- Transportation: $2,667 (vehicles + insurance + gas)
- Gambling: $2,100 (Jane's DraftKings)
- Groceries: ~$2,100
- Utilities: ~$900
- Dining: ~$900
[... more categories ...]

Jane's gambling represents 13.1% of net income ($2,100 / $16,000)
```

**Learning Points**:
- Agents categorize expenses automatically
- Can calculate percentages and ratios
- Interactive follow-up questions provide deeper insights

### Exercise 4: Cash Flow Analysis

**Objective**: Identify months with the lowest account balances

**Steps**:

1. Type: `@cashflow-analyst identify months with risky low balances`
2. Review the analysis
3. Ask: "What's the pattern between payday and low balances?"

**Expected Result**:
- List of minimum balance by month
- Identification of which weeks are tightest
- Pattern: Balances lowest just before payday (around the 14th)
- Recommendation to build cash buffer

**Learning Points**:
- Timing of income vs. expenses matters
- Bi-monthly pay can create cash flow challenges
- Proactive analysis prevents overdrafts

### Exercise 5: Budget Compliance

**Objective**: Evaluate budget health using the 50/30/20 rule

**Steps**:

1. Type: `@budget-monitor evaluate budget against 50/30/20 rule`
2. Review the breakdown
3. Ask: "What's the biggest area of concern?"

**Expected Result**:
```
50/30/20 Rule Analysis:
Needs (50%): 62% ❌ (over budget)
  - Housing: 27%
  - Transportation: 11%
  - Insurance: 9%
  - Utilities: 4%
  - Groceries: 8%
  - Other: 3%

Wants (30%): 28% ✓
  - Dining: 6%
  - Gambling: 9%
  - Entertainment: 5%
  - Shopping: 8%

Savings (20%): 10% ❌ (under target)

Recommendation: Needs are over budget. Consider refinancing mortgage
or reducing transportation costs. Gambling expenses are concerning.
```

**Learning Points**:
- Agents apply financial frameworks automatically
- Visual feedback (✓/❌) makes issues clear
- Prioritized recommendations guide action

### Exercise 6: Savings Progress

**Objective**: Track savings growth and interest earned in 2024

**Steps**:

1. Type: `@savings-tracker calculate total interest earned in 2024`
2. Review the monthly progression
3. Ask: "Project savings balance for next 3 years"

**Expected Result**:
```
2024 Savings Summary:
Starting Balance: $8,500
Ending Balance: $14,250
Total Contributions: $6,000 (12 × $500)
Total Interest: ~$450
Effective APY: 4.25%

Projections (assuming same contribution rate):
2025: $20,850
2026: $27,600
2027: $34,500

Current savings rate: 3.75% of gross income
Recommended: 15-20%
```

**Learning Points**:
- Agents track progress over time
- Can project future based on current patterns
- Compares actual vs. recommended savings rates

### Exercise 7: Retirement Analysis

**Objective**: Compare Bob's 401(k) and Jane's 403(b) performance

**Steps**:

1. Type: `@retirement-analyzer compare Bob and Jane's retirement accounts`
2. Review the performance analysis
3. Ask: "At this rate, how much will they have at retirement?"

**Expected Result**:
```
Retirement Account Comparison:

Bob's 401(k) (Fidelity):
  Starting: $142,500
  Ending: $169,162
  Growth: $26,662 (18.7%)
  Contributions: ~$14,250
  Investment Gains: ~$12,412
  Rate of Return: ~8.7%

Jane's 403(b) (TIAA):
  Starting: $98,750
  Ending: $116,447
  Growth: $17,697 (17.9%)
  Contributions: ~$9,750
  Investment Gains: ~$7,947
  Rate of Return: ~8.0%

Both accounts are performing well. Bob's has higher absolute growth
due to larger starting balance. Similar return rates suggest good
fund selections in both accounts.

Retirement Projection (age 67):
Bob: ~$765,000 (20 years)
Jane: ~$485,000 (22 years)
Combined: ~$1,250,000

Assumes 7% average annual return and current contribution levels.
```

**Learning Points**:
- Agents can read complex financial documents
- Calculates returns and projects future values
- Provides actionable retirement planning insights

### Exercise 8: Tax Verification

**Objective**: Verify 2023 tax return accuracy

**Steps**:

1. Type: `@tax-verifier verify 2023 Form 1040`
2. Review the verification
3. Ask: "Does the interest income match the savings statements?"

**Expected Result**:
```
2023 Form 1040 Verification:

✓ W-2 Income: $160,000 ($95k + $65k)
✓ Interest Income: $340 (matches savings account total)
✓ Standard Deduction: $27,700 (correct for MFJ)
✓ Taxable Income: $132,640
✓ Tax Calculation: $15,318 (verified against 2023 brackets)
✓ Federal Withholding: $16,500
✓ Refund: $1,182

All calculations verified. Tax return appears accurate.
```

**Learning Points**:
- Agents can verify complex tax calculations
- Cross-references multiple data sources
- Provides confidence in tax filing accuracy

## Part 4: Advanced Workflows

### Workflow 1: Monthly Financial Review

**Goal**: Complete financial health check for a specific month

```
1. @document-checker verify [month] files present
2. @financial-auditor audit [month] for errors
3. @spending-analyzer breakdown [month] spending
4. @cashflow-analyst review [month] cash flow
```

**Use Case**: Monthly routine to stay on top of finances

### Workflow 2: Annual Financial Summary

**Goal**: Year-end comprehensive financial analysis

```
1. @document-checker verify all 2024 files
2. @spending-analyzer analyze entire year spending trends
3. @budget-monitor evaluate full year against budget
4. @savings-tracker calculate year-end savings progress
5. @retirement-analyzer review retirement account performance
6. @tax-verifier prepare for tax season
```

**Use Case**: Annual review for tax prep and financial planning

### Workflow 3: Problem Investigation

**Goal**: Investigate a specific concern (e.g., "Why was our balance so low in March?")

```
1. @cashflow-analyst identify March cash flow issues
2. @spending-analyzer show March spending anomalies
3. @financial-auditor verify March calculations
4. Follow-up questions to drill down
```

**Use Case**: Ad-hoc investigation of financial concerns

### Workflow 4: Financial Planning

**Goal**: Plan for major purchase or life change

```
1. @budget-monitor current spending baseline
2. @cashflow-analyst identify available cash
3. @savings-tracker project savings growth
4. @retirement-analyzer ensure retirement on track
5. Calculate affordability of new expense
```

**Use Case**: Decision support for major financial decisions

## Part 5: Creating Your Own Agents

### Agent Design Principles

1. **Single Responsibility**: Each agent should have one clear purpose
2. **Clear Objectives**: Define what success looks like
3. **Specific Instructions**: Tell the agent exactly what to analyze
4. **Context Provision**: Include relevant background information
5. **Output Format**: Specify how results should be presented

### Example: Creating a "Debt Reduction Planner" Agent

**File**: `.claude/agents/debt-planner.md`

```markdown
You are a debt reduction specialist. Analyze Bob and Jane's financial
documents and create a personalized debt reduction plan:

1. Identify all debt obligations (mortgage, vehicle loans)
2. Calculate total monthly debt payments
3. Determine debt-to-income ratio
4. Analyze extra cash available for debt paydown
5. Create a debt snowball or avalanche strategy
6. Project debt-free timeline under different scenarios

Financial Context:
- Mortgage: $2,215/month
- Ford F-150: $504/month
- Harley Davidson: $385/month
- Combined income: $160,000/year

Provide a clear action plan with timelines and projected savings.
```

**Usage**: `@debt-planner create debt reduction strategy`

### Agent Template

```markdown
You are a [role/specialty]. [Primary objective]:

[Numbered list of specific tasks to perform]

[Context section with relevant background information]

[Output format instructions]
```

## Part 6: Teaching This to Others

### Workshop Outline (2 hours)

**Part 1: Introduction (15 min)**
- What is Claude Code?
- What are agents?
- Why use AI for financial analysis?

**Part 2: Demo (30 min)**
- Live demonstration of document-checker
- Live demonstration of spending-analyzer
- Show the power of instant insights

**Part 3: Hands-On (60 min)**
- Participants run exercises 1-4
- Guide them through agent invocation
- Help with questions

**Part 4: Discussion (15 min)**
- What other use cases can you think of?
- How could this apply to your work?
- Q&A

### Key Talking Points

1. **Speed**: "What would take hours manually takes seconds with agents"
2. **Accuracy**: "Agents don't make arithmetic errors or miss details"
3. **Consistency**: "Same analysis approach every time"
4. **Scalability**: "Analyze 10 files or 1,000 files with the same effort"
5. **Accessibility**: "No programming required to create powerful analysis tools"

### Common Questions

**Q: Can agents make mistakes?**
A: Yes, always verify critical calculations. Agents are tools to assist, not replace, human judgment.

**Q: Do I need programming knowledge?**
A: No! Agents are defined in simple markdown files with plain English instructions.

**Q: Can I use this with my real financial data?**
A: Absolutely! Replace the sample data with your own documents. Keep data privacy in mind.

**Q: How much does Claude Code cost?**
A: See pricing at claude.ai/code. Consider cost vs. value of time saved.

**Q: Can agents work with other document types?**
A: Yes! Agents can analyze any file type Claude Code supports (PDFs, spreadsheets, text files, etc.)

## Part 7: Next Steps

### Expand the Project

1. **Add more agents**:
   - Investment Portfolio Analyzer
   - Credit Score Impact Estimator
   - Emergency Fund Tracker
   - Insurance Coverage Reviewer

2. **Generate more data**:
   - Run the Python scripts to generate different years
   - Modify scripts to simulate different scenarios
   - Create "what-if" scenarios

3. **Create visualizations**:
   - Export agent output to spreadsheets
   - Create charts and graphs
   - Build dashboards

4. **Build automation**:
   - Schedule regular agent runs
   - Create monthly report templates
   - Set up alerts for unusual patterns

### Apply to Other Domains

**Legal Document Analysis**:
- Contract reviewer agent
- Compliance checker agent
- Risk assessment agent

**Healthcare Records**:
- Medical history analyzer
- Medication interaction checker
- Test results tracker

**Business Operations**:
- Sales pipeline analyzer
- Customer churn predictor
- Inventory optimizer

**Academic Research**:
- Literature review agent
- Data quality checker
- Citation verifier

## Part 8: Resources

### Documentation

- **Claude Code Docs**: [claude.ai/code/docs](https://claude.ai/code/docs)
- **Agent Creation Guide**: See `.claude/agents/` examples
- **Sample Data Source**: data/bobandjanedoe/ directory

### Source Files

- **Agent Definitions**: `.claude/agents/*.md`
- **Financial Data**: `data/bobandjanedoe/statements/`
- **Data Generators**: `data/bobandjanedoe/generate_*.py`
- **Original Documentation**: `data/bobandjanedoe/README.md`

### Community

- Share your custom agents
- Contribute improvements
- Report issues and suggestions

## Conclusion

You now have a complete framework for demonstrating Claude Code and agents using realistic financial analysis scenarios. This tutorial shows that AI is not just for programmers—anyone can create powerful analysis tools with simple, clear instructions.

**Key Takeaways**:

1. Agents make AI accessible to non-programmers
2. Specialized agents outperform generalist approaches
3. Real-world applications provide best demonstrations
4. The possibilities are limited only by imagination

**Ready to get started? Try this:**

```
@document-checker verify all files are present
```

Welcome to the future of AI-assisted analysis!

---

**Questions or Feedback?**
- Review the agent definitions in `.claude/agents/`
- Experiment with different prompts
- Create your own custom agents
- Share what you learn!
