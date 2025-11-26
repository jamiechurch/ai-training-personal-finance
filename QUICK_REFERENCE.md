# Quick Reference Guide

## Available Agents

### 1. @document-checker
**Verify all files are present**
```
@document-checker verify all files are present
@document-checker list all checking statements
```

### 2. @financial-auditor
**Cross-reference and verify accuracy**
```
@financial-auditor audit January 2024
@financial-auditor check utility bills vs bank statements
@financial-auditor verify interest calculations
```

### 3. @spending-analyzer
**Analyze spending patterns**
```
@spending-analyzer analyze Q1 2024 spending
@spending-analyzer show gambling expenses trend
@spending-analyzer compare March vs April spending
@spending-analyzer find cost-cutting opportunities
```

### 4. @cashflow-analyst
**Track money in vs out**
```
@cashflow-analyst identify risky low balance months
@cashflow-analyst analyze bi-monthly paycheck impact
@cashflow-analyst show 2024 cash flow trends
```

### 5. @budget-monitor
**Evaluate budget health**
```
@budget-monitor evaluate against 50/30/20 rule
@budget-monitor identify overspending categories
@budget-monitor compare to national averages
```

### 6. @savings-tracker
**Monitor savings progress**
```
@savings-tracker calculate total interest earned in 2024
@savings-tracker project savings for next 3 years
@savings-tracker verify monthly transfer goals
```

### 7. @retirement-analyzer
**Evaluate retirement accounts**
```
@retirement-analyzer compare Bob and Jane's accounts
@retirement-analyzer calculate rate of return
@retirement-analyzer project retirement readiness
```

### 8. @tax-verifier
**Verify tax return accuracy**
```
@tax-verifier verify 2023 Form 1040
@tax-verifier check interest income calculation
@tax-verifier validate tax bracket calculations
```

## Common Workflows

### Monthly Review
```
@document-checker verify [month] files
@financial-auditor audit [month]
@spending-analyzer show [month] spending
@cashflow-analyst review [month] cash flow
```

### Annual Summary
```
@spending-analyzer analyze full year trends
@savings-tracker calculate year-end progress
@retirement-analyzer review annual performance
@budget-monitor evaluate full year budget
```

### Problem Investigation
```
@cashflow-analyst identify [month] cash flow issues
@spending-analyzer show [month] anomalies
@financial-auditor verify [month] calculations
```

## File Locations

- **Agents**: `.claude/agents/*.md`
- **Data**: `data/bobandjanedoe/statements/`
- **Tutorial**: `TUTORIAL.md`
- **Examples**: `examples/SAMPLE_ANALYSIS.md`

## Quick Stats - Bob & Jane Doe

- **Combined Income**: $160K/year (~$13.3K/month gross)
- **Net Income**: ~$9,672/month
- **Major Expenses**:
  - Mortgage: $2,215/mo
  - Vehicles: $889/mo
  - Insurance: $743/mo
  - Gambling: $700/mo
- **Savings**: $500/mo to HYSA
- **Retirement**: Bob 401(k) $169K, Jane 403(b) $116K

## Tips

1. **Be specific**: "analyze January" not "analyze data"
2. **Ask follow-ups**: Agents can drill deeper
3. **Cross-reference**: Use multiple agents for verification
4. **Export data**: Ask agents to create tables/CSV format

## Getting Help

- Full tutorial: `TUTORIAL.md`
- Example outputs: `examples/SAMPLE_ANALYSIS.md`
- Data info: `data/bobandjanedoe/README.md`
