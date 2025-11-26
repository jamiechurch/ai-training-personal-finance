# Sample Financial Data

This project demonstrates Claude Code agents using financial analysis examples. To use the agents, you can either use your own financial data or download sample data.

## Option 1: Use Your Own Data (Recommended)

Place your financial documents (PDFs, CSVs, etc.) in the `data/` folder and run the agents on your own files.

Example:
```
data/
├── bank_statements/
├── credit_card/
├── investment_accounts/
└── tax_documents/
```

Then run agents like:
```
@spending-analyzer analyze my spending patterns
@cashflow-analyst review my cash flow
```

## Option 2: Download Sample Data (For Learning)

If you want to practice with the fictional "Bob and Jane Doe" financial data used in the tutorial:

1. **Clone the sample data repository:**
   ```bash
   git clone https://github.com/jamiechurch/bobandjanedoe.git data/bobandjanedoe
   ```

2. **Verify the data:**
   ```bash
   # Mac/Linux
   find data/bobandjanedoe/statements -name "*.pdf" | wc -l

   # Windows
   dir data\bobandjanedoe\statements /s /b | find /c ".pdf"
   ```

   You should see 75 PDF files.

3. **Start analyzing:**
   ```
   @spending-analyzer analyze Q1 2024 spending
   ```

## Sample Data Contents (Bob & Jane Doe)

The sample repository contains 75 fictional financial documents:
- 12 checking account statements (2024)
- 12 savings account statements (2024)
- 2 retirement statements (401k, 403b)
- 1 tax return (Form 1040)
- 48 utility bills (electric, gas, water, internet)

**Note**: All data is completely fictional and generated for educational purposes.

## Generating Your Own Sample Data

The bobandjanedoe repository includes Python scripts to generate financial PDFs if you want to create custom scenarios:

```bash
cd data/bobandjanedoe
python generate_statements.py
python generate_savings_statements.py
python generate_retirement_statements.py
python generate_tax_return.py
python generate_utility_bills.py
```

See the [bobandjanedoe README](https://github.com/jamiechurch/bobandjanedoe) for details.
