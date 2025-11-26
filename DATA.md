# Sample Financial Data

**Good news: Sample data is already included!**

This repository comes with realistic financial data ready for analysis. No downloads needed - just clone and start analyzing.

---

## What's Included

The `data/` folder contains **27 sample financial PDFs** from the fictional "Bob & Jane Doe" household:

### File Structure

```
data/
├── checking/
│   └── 12 monthly checking account statements (Jan-Dec 2024)
├── savings/
│   └── 12 monthly savings account statements (Jan-Dec 2024)
├── investments/
│   ├── Bob_Retirement_401k_2024.pdf
│   └── Jane_Retirement_403b_2024.pdf
└── taxes/
    └── Form_1040_2023.pdf
```

### Quick Summary

- **12 checking statements**: Monthly Bank of America statements showing income and expenses
- **12 savings statements**: Monthly savings account activity and interest
- **2 retirement statements**: 401(k) and 403(b) accounts with contributions and performance
- **1 tax return**: 2023 Form 1040 with complete financial picture

**Total: 27 PDF files**

---

## About Bob & Jane Doe

The sample data represents a fictional dual-income household:

- **Bob**: Tech worker with 401(k), drives a Ford F-150
- **Jane**: Public sector employee with 403(b), rides a Harley Davidson
- **Combined income**: ~$160,000/year
- **Financial habits**: Good savers (38% rate) but with some concerning patterns (gambling expenses)

All data is completely fictional and generated for educational purposes. No real financial information is used.

---

## Using the Sample Data

**No setup required!** After cloning the repository, you can immediately run:

```bash
claude
@spending-analyzer analyze Q1 2024 spending
@cashflow-analyst identify risky months
@budget-monitor evaluate against 50/30/20 rule
@retirement-analyzer compare Bob and Jane's accounts
```

The agents will automatically find and analyze the PDF files in the `data/` folder.

---

## Using Your Own Data

Want to analyze your own financial documents instead?

### Option 1: Replace Sample Data

1. **Remove sample files** (or move them to a backup folder):
   ```bash
   mv data data_samples_backup
   mkdir data
   ```

2. **Add your own PDFs**:
   ```bash
   cp ~/Documents/MyBankStatements/*.pdf data/
   ```

3. **Start analyzing**:
   ```bash
   @spending-analyzer analyze my recent spending
   ```

### Option 2: Add to Sample Data

Keep the samples and add your own files:

```bash
mkdir data/my_statements
cp ~/Documents/MyBankStatements/*.pdf data/my_statements/
```

Then specify which files to analyze:
```
@spending-analyzer analyze documents in data/my_statements
```

### Supported File Types

The agents work with any financial PDFs:
- Bank statements (checking, savings, credit card)
- Investment account statements
- Retirement account statements (401k, 403b, IRA)
- Tax returns (Form 1040, W-2, 1099)
- Utility bills
- Loan statements
- Mortgage statements

---

## File Organization Tips

**Recommended structure for your own data:**

```
data/
├── bank/
│   ├── checking/
│   └── credit_cards/
├── investments/
│   ├── retirement/
│   └── brokerage/
├── taxes/
│   ├── 2023/
│   └── 2024/
└── bills/
    ├── utilities/
    └── insurance/
```

This makes it easier to target specific analyses:
```
@spending-analyzer analyze data/bank/checking
@retirement-analyzer review data/investments/retirement
```

---

## Sample Data Details

### Checking Account Highlights

- **Monthly income**: ~$9,600 (Bob & Jane combined)
- **Major expenses**: Mortgage ($2,215), vehicle loans ($889), utilities
- **Interesting pattern**: Gambling expenses (~$700/month)
- **Balance trends**: Lowest mid-month between paychecks

### Savings Account Highlights

- **Starting balance**: ~$15,000
- **Monthly contributions**: $1,000-$3,000
- **Interest earned**: ~$30/month
- **Growth**: Strong upward trend

### Retirement Accounts

- **Bob's 401(k)**: ~$125,000 balance, aggressive growth portfolio
- **Jane's 403(b)**: ~$95,000 balance, balanced portfolio
- **Combined contributions**: ~$2,000/month
- **Employer match**: Both receiving full match

### Tax Return (2023)

- **Filing status**: Married Filing Jointly
- **Total income**: ~$156,000
- **Federal tax**: ~$18,000
- **Refund**: ~$2,500

---

## Privacy & Security

**Using your own data safely:**

- All analysis happens **locally** on your computer
- PDFs are read but never uploaded or shared
- Consider using **anonymized copies** of sensitive documents
- Remove account numbers from filenames
- Never commit real financial data to public GitHub repositories

**Best practice**: Keep a separate folder for sensitive documents:
```bash
# Keep real data outside the repository
~/Documents/MyFinances/  # Your real data (not in git)
~/Documents/AI-Training-Personal-Finance/data/  # Sample data only (in git)
```

---

## What Makes This Data Realistic?

The sample PDFs were carefully designed to include:

- **Authentic formatting**: Matches real bank statement layouts
- **Realistic transactions**: Grocery stores, gas stations, mortgage payments
- **Consistent patterns**: Same merchants appearing regularly
- **Financial complexity**: Multiple income sources, various expense categories
- **Real-world challenges**: Tight cash flow, concerning spending patterns
- **Complete picture**: Checking, savings, retirement, and taxes

This makes the agents' analyses meaningful and demonstrates their real-world capabilities.

---

## Questions?

**Where are the files?**
Check the `data/` folder after cloning. You should see subdirectories for checking, savings, investments, and taxes.

**Can I delete the sample data?**
Yes! Replace it with your own financial documents anytime.

**How do I verify the data is there?**
```bash
# Mac/Linux
find data -name "*.pdf" | wc -l

# Windows
dir data /s /b | find /c ".pdf"
```
Should show 27 PDF files.

**Can I use CSV or Excel files?**
The agents are optimized for PDF analysis, but you can try other formats. Results may vary.

---

**Ready to analyze?** The sample data is waiting for you!

```bash
claude
@spending-analyzer analyze Q1 2024 spending
```

Let's explore Bob & Jane's finances together!
