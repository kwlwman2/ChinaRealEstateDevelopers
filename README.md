# China Real Estate Developers - What were Their Common Financial Tricks

### Introduction
This project is to explore Chinese real estate developers' financial statement data and uncover what were the common tricks they leveraged to cover up their high debt loads on their financial statements before the Three Red Lines policy was enforced by the central government in the Aug of 2020. For more details about the project and analysis, you can also read my article posted on the Medium https://medium.com/@diguoxiongfeng/china-real-estate-developers-what-were-their-common-financial-tricks-235df28572f9

### Built with
- Python Pandas
- Python NumPy
- Python Matplotlib

### This project is divided in the following key sections:
- Data exploration with data visualization
- Data preprocessing & cleanning
- Solve the following three major questions 
  - Q1: Market Concentration Analysis — How was the entire real estate market changing over the three-year period.
  - Q2: What kind of common “financial engineering” developers were leveraging to polish up their real financial position.
  - Q3: Can we create a model that can help us to pick up the best 5 and worst 5 companies, and long top 5 and short worst 5 to see how this pseudo portfolio performs in the next 6–9 month returns (from 2020/3/31–2020/12/31)?
- Summary & Takeaways

### Code and data

*  `China_Real_Estate_Firms_Financial_Analysis.ipynb` - Python Jupyter notebook for Financial Analysis
* `Property_Developers-_Financial_Data.xlsx` - raw data containing 116 listed real estate developers, with three-year accounting data spanning from 2017 to 2019

### Here is the schema and explanation of each variable in the files:

* Sec_Code: the security code of a listed real estate developer.
* Sec_Name: the company name
* Cash_From_Customers: how much cash proceeds have been received from customers. This is a key indicator to evaluate a developer’s sales & marketing ability to drive sales. To give you a heads-up. In China, some customers buy a new property that is still in construction and will be completed within 1 or 2 years. Typically speaking, another important alternative indicator called contract sales would be used to analyze cash received from customers, but this dataset does not cover it.
* NetCF_from_Operating: cash flow from net operating activity
* NetCF_fromInvesting: cash flow received from investing activity 
* Proceeds_FromBorrowing: how much cash received from borrowers Proceeds_FromBondIssues: how much * cash was received from issuing bonds 
* Dividend&InterestPaid: how much dividend a real estate developer has distributed in a fiscal year
* NetCF_from_Financing: how much cash received from financing activities
* Provision_InventoryDepreciation: provision charged on the unsold property. This is an interesting indicator. Typically if a newly built property cannot be sold, it will be counted as an inventory unit on the accounting book and depreciation provision rules will be applied. A good real estate developer should have a high turnover to sell newly built properties as soon as possible to avoid such non-cash charges.
* Operating_Revenue: how much revenues generated through core business activity
* Bills_Payable: any bills that are payable to banks or other financial institutions. Usually, bills payable are short-term debt
* A/C_Payable: short term debt to suppliers
* Total_CI: total comprehensive income
* CI_For_Non_Controlling_Ints: comprehensive income for non-controlling interests
* NonControling_Interests: non-controlling interests from minority shareholders in total equity
* Total_Equity: total equity on the shareholders’ equity statement

### Takeaways

With the analysis of China real estate developers, we can get a few takeaways:

1. As the economy was trending down (China was inflicted by the trade war against the United States and then COVID-19, the winner will be much stronger with greater access to external financing to bid land resources.

2. Payables are a common tool that developers leverage in order to improve their financial well-being in the short term.

3. We can infer joint venture financing through the ratios between comprehensive income attributed to non-controlling interests and non-controlling interest to total equity. These two ratios’ trends should be aligned if no joint venture financing is involved. Companies with strong balance sheets typically would not opt for such financing sources as this type of joint venture financing has a higher cost of borrowing, but weaker players tend to do so.

4. Even though we know which signals are good or bad, it is still very hard to leverage those signals to develop a profitable trading model even in paper trading. If a trading idea cannot pass paper trading, just don’t even think about the real trading environment.

5. Obviously, our trading ideas do not include any rebalancing techniques. Given the market situation, our trade model can be improved through rebalancing. For example, we can rebalance our portfolio based on the latest financial statement, such as selling stocks that fall out of Quantile Bin 1 and buying stocks back if they get out of Quantile bin 5 and so on.


### Acknowledgement
Thank you so much for my wife to support my career and our family.

