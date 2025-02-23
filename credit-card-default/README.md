# Credit Card Default Dataset

http://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients

This research employed a binary variable, default payment (Yes = 1, No = 0), as the response variable. This study reviewed the literature and used the following 23 variables as explanatory variables:

* LIMIT_BAL: Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit.
* SEX: Gender (1 = male; 2 = female).
* EDUCATION: Education (1 = graduate school; 2 = university; 3 = high school; 4 = others).
* MARRIAGE: Marital status (1 = married; 2 = single; 3 = others).
* AGE: Age (year).
* PAY 1-6 : History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows: X6 = the repayment status in September, 2005; X7 = the repayment status in August, 2005; . . .;X11 = the repayment status in April, 2005. The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.
* BILL_AMT 1-6: Amount of bill statement (NT dollar). X12 = amount of bill statement in September, 2005; X13 = amount of bill statement in August, 2005; . . .; X17 = amount of bill statement in April, 2005.
* PAY_AMT 1-6: Amount of previous payment (NT dollar). X18 = amount paid in September, 2005; X19 = amount paid in August, 2005; . . .;X23 = amount paid in April, 2005.
* DEFAULT: If they defaulted on the next payment or not (1 - yes, 0 - no)

## Simple DataSet

[Link to Simple Dataset](./default-simple.csv)

| id | balance | sex | education | marriage | age | default |
|----|---------|-----|-----------|----------|-----|---------|
| 1  | 20000   | 2   | 2         | 1        | 24  | 0       |
| 2  | 120000  | 2   | 2         | 2        | 26  | 0       |
| 3  | 90000   | 2   | 2         | 2        | 34  | 1       |
| 4  | 50000   | 2   | 2         | 1        | 37  | 1       |
| 5  | 50000   | 1   | 2         | 1        | 57  | 1       |
| 6  | 50000   | 1   | 1         | 2        | 37  | 1       |
| 7  | 500000  | 1   | 1         | 2        | 29  | 1       |
| 8  | 100000  | 2   | 2         | 2        | 23  | 1       |
| 9  | 140000  | 2   | 3         | 1        | 28  | 1       |
| 10 | 20000   | 1   | 3         | 2        | 35  | 1       |
| 11 | 200000  | 2   | 3         | 2        | 34  | 1       |
| 12 | 260000  | 2   | 1         | 2        | 51  | 1       |
| 13 | 630000  | 2   | 2         | 2        | 41  | 1       |
| 14 | 70000   | 1   | 2         | 2        | 30  | 0       |
| 15 | 250000  | 1   | 1         | 2        | 29  | 1       |
| 16 | 50000   | 2   | 3         | 3        | 23  | 1       |
| 17 | 20000   | 1   | 1         | 2        | 24  | 0       |
| 18 | 320000  | 1   | 1         | 1        | 49  | 1       |
| 19 | 360000  | 2   | 1         | 1        | 49  | 1       |
| 20 | 180000  | 2   | 1         | 2        | 29  | 1       |
| 21 | 130000  | 2   | 3         | 2        | 39  | 1       |
| 22 | 120000  | 2   | 2         | 1        | 39  | 0       |

## Longer Dataset

[Link to Simple Dataset in CSV](./default.csv)

[Link to Simple Dataset in EXCEL](./default.xls)

```text
| ID | LIMIT_BAL | SEX | EDUCATION | MARRIAGE | AGE | PAY_0 | PAY_2 | PAY_3 | PAY_4 | PAY_5 | PAY_6 | BILL_AMT1 | BILL_AMT2 | BILL_AMT3 | BILL_AMT4 | BILL_AMT5 | BILL_AMT6 | PAY_AMT1 | PAY_AMT2 | PAY_AMT3 | PAY_AMT4 | PAY_AMT5 | PAY_AMT6 | default |
|----|-----------|-----|-----------|----------|-----|-------|-------|-------|-------|-------|-------|-----------|-----------|-----------|-----------|-----------|-----------|----------|----------|----------|----------|----------|----------|---------|
| 1  | 20000     | 2   | 2         | 1        | 24  | 2     | 2     | -1    | -1    | -2    | -2    | 3913      | 3102      | 689       | 0         | 0         | 0         | 0        | 689      | 0        | 0        | 0        | 0        | 1       |
| 2  | 120000    | 2   | 2         | 2        | 26  | -1    | 2     | 0     | 0     | 0     | 2     | 2682      | 1725      | 2682      | 3272      | 3455      | 3261      | 0        | 1000     | 1000     | 1000     | 0        | 2000     | 1       |
| 3  | 90000     | 2   | 2         | 2        | 34  | 0     | 0     | 0     | 0     | 0     | 0     | 29239     | 14027     | 13559     | 14331     | 14948     | 15549     | 1518     | 1500     | 1000     | 1000     | 1000     | 5000     | 0       |
| 4  | 50000     | 2   | 2         | 1        | 37  | 0     | 0     | 0     | 0     | 0     | 0     | 46990     | 48233     | 49291     | 28314     | 28959     | 29547     | 2000     | 2019     | 1200     | 1100     | 1069     | 1000     | 0       |
| 5  | 50000     | 1   | 2         | 1        | 57  | -1    | 0     | -1    | 0     | 0     | 0     | 8617      | 5670      | 35835     | 20940     | 19146     | 19131     | 2000     | 36681    | 10000    | 9000     | 689      | 679      | 0       |
| 6  | 50000     | 1   | 1         | 2        | 37  | 0     | 0     | 0     | 0     | 0     | 0     | 64400     | 57069     | 57608     | 19394     | 19619     | 20024     | 2500     | 1815     | 657      | 1000     | 1000     | 800      | 0       |
| 7  | 500000    | 1   | 1         | 2        | 29  | 0     | 0     | 0     | 0     | 0     | 0     | 367965    | 412023    | 445007    | 542653    | 483003    | 473944    | 55000    | 40000    | 38000    | 20239    | 13750    | 13770    | 0       |
| 8  | 100000    | 2   | 2         | 2        | 23  | 0     | -1    | -1    | 0     | 0     | -1    | 11876     | 380       | 601       | 221       | -159      | 567       | 380      | 601      | 0        | 581      | 1687     | 1542     | 0       |
| 9  | 140000    | 2   | 3         | 1        | 28  | 0     | 0     | 2     | 0     | 0     | 0     | 11285     | 14096     | 12108     | 12211     | 11793     | 3719      | 3329     | 0        | 432      | 1000     | 1000     | 1000     | 0       |
| 10 | 20000     | 1   | 3         | 2        | 35  | -2    | -2    | -2    | -2    | -1    | -1    | 0         | 0         | 0         | 0         | 13007     | 13912     | 0        | 0        | 0        | 13007    | 1122     | 0        | 0       |
| 11 | 200000    | 2   | 3         | 2        | 34  | 0     | 0     | 2     | 0     | 0     | -1    | 11073     | 9787      | 5535      | 2513      | 1828      | 3731      | 2306     | 12       | 50       | 300      | 3738     | 66       | 0       |
| 12 | 260000    | 2   | 1         | 2        | 51  | -1    | -1    | -1    | -1    | -1    | 2     | 12261     | 21670     | 9966      | 8517      | 22287     | 13668     | 21818    | 9966     | 8583     | 22301    | 0        | 3640     | 0       |
| 13 | 630000    | 2   | 2         | 2        | 41  | -1    | 0     | -1    | -1    | -1    | -1    | 12137     | 6500      | 6500      | 6500      | 6500      | 2870      | 1000     | 6500     | 6500     | 6500     | 2870     | 0        | 0       |
| 14 | 70000     | 1   | 2         | 2        | 30  | 1     | 2     | 2     | 0     | 0     | 2     | 65802     | 67369     | 65701     | 66782     | 36137     | 36894     | 3200     | 0        | 3000     | 3000     | 1500     | 0        | 1       |
| 15 | 250000    | 1   | 1         | 2        | 29  | 0     | 0     | 0     | 0     | 0     | 0     | 70887     | 67060     | 63561     | 59696     | 56875     | 55512     | 3000     | 3000     | 3000     | 3000     | 3000     | 3000     | 0       |
| 16 | 50000     | 2   | 3         | 3        | 23  | 1     | 2     | 0     | 0     | 0     | 0     | 50614     | 29173     | 28116     | 28771     | 29531     | 30211     | 0        | 1500     | 1100     | 1200     | 1300     | 1100     | 0       |
| 17 | 20000     | 1   | 1         | 2        | 24  | 0     | 0     | 2     | 2     | 2     | 2     | 15376     | 18010     | 17428     | 18338     | 17905     | 19104     | 3200     | 0        | 1500     | 0        | 1650     | 0        | 1       |
| 18 | 320000    | 1   | 1         | 1        | 49  | 0     | 0     | 0     | -1    | -1    | -1    | 253286    | 246536    | 194663    | 70074     | 5856      | 195599    | 10358    | 10000    | 75940    | 20000    | 195599   | 50000    | 0       |
| 19 | 360000    | 2   | 1         | 1        | 49  | 1     | -2    | -2    | -2    | -2    | -2    | 0         | 0         | 0         | 0         | 0         | 0         | 0        | 0        | 0        | 0        | 0        | 0        | 0       |
| 20 | 180000    | 2   | 1         | 2        | 29  | 1     | -2    | -2    | -2    | -2    | -2    | 0         | 0         | 0         | 0         | 0         | 0         | 0        | 0        | 0        | 0        | 0        | 0        | 0       |
| 21 | 130000    | 2   | 3         | 2        | 39  | 0     | 0     | 0     | 0     | 0     | -1    | 38358     | 27688     | 24489     | 20616     | 11802     | 930       | 3000     | 1537     | 1000     | 2000     | 930      | 33764    | 0       |
| 22 | 120000    | 2   | 2         | 1        | 39  | -1    | -1    | -1    | -1    | -1    | -1    | 316       | 316       | 316       | 0         | 632       | 316       | 316      | 316      | 0        | 632      | 316      | 0        | 1       |
| 23 | 70000     | 2   | 2         | 2        | 26  | 2     | 0     | 0     | 2     | 2     | 2     | 41087     | 42445     | 45020     | 44006     | 46905     | 46012     | 2007     | 3582     | 0        | 3601     | 0        | 1820     | 1       |
```

