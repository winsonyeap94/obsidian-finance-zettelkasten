---
tags: 
creation-date: 2024-07-16 20:26
---
## CFA - Forecasting Asset Class Returns

>[!info] Learning Outcome Statements
>1. Discuss approaches to setting expectations for **fixed-income returns**.
>2. Discuss **risks** faced by investors in emerging market fixed-income securities and the **country risk analysis techniques** used to evaluate emerging market economies.
>3. Discuss approaches to setting expectations for **equity investment market returns**.
>4. Discuss risks faced by investors in **emerging market equity securities**.
>5. Explain how economic and competitive factors can affect expectations for **real estate investment markets** and sector returns.
>6. Discuss major approaches to **forecasting exchange rates**.
>7. Discuss methods of **forecasting volatility**.
>8. Recommend and justify **changes in the component weights** of a global investment portfolio based on trends and expected changes in macroeconomic factors.

> [!recap]- Brief Recap...
> - Metrics such as asset prices, volatilities, risk premiums, etc. show **persistence**, **momentum**, and **clustering** in the short term.
> - They **converge** to levels consistent with **economic and financial fundamentals** over long enough horizons.
> - **Time horizons** are key in forecasting.
> 
> ![[Pasted image 20240716203636.png|500]]
> 
> High-level approaches to forecasting:
> 1. Formal tools
> 	- Proven research methods that allow for precise definition and independent replication of findings.
> 	- Include *statistical methods*, *discounted cash flow models*, and *risk premium models*.
> 2. Surveys
> 	- Seek expert opinions.
> 3. Judgment
> 	- Subjective processing of information obtained from different sources.

## Forecasting Fixed-Income Returns

### Main approaches for forecasting fixed-income returns
--- start-multi-column: ID_cjqf
```column-settings
Number of Columns: 3
Largest Column: standard
```

**Discounted cash flow**

![[Pasted image 20240716204517.png|300]]
- Involves mapping out the *future inflows and outflows of cash* associated with the investment and discounting them to obtain a present value.

--- column-break ---

**Risk premium approach**

![[Pasted image 20240716204600.png|300]]
- Involves *starting with a risk-free rate of interest* and *adding up compensation* for risks as required by the investor.

--- column-break ---

**Equilibrium models**

![[Pasted image 20240716204755.png|300]]
- Provides consistency across asset classes by setting an *expectation relative to other asset class performances*.

--- end-multi-column
#### (1) Discounted Cashflow Models (DCF)
- Most fixed-income securities have finite maturities with:
	- *Known cash flows*, or
	- Cash flows which can be *modelled accurately*.
	make DCF useful in forecasting fixed-income returns.
- Most *precise* method.
- DCF models incorporate projections of how cash flows and rates will evolve over the investment horizon.
- The **yield to maturity (YTM)** is used as the estimate for the expected return.
	- YTM is the rate that <mark style="background: #FFF3A3A6;">equates the present value of future cash flows to the current price of the security</mark>.
	- It is calculated as an average of YTM of individual bonds.
- Realised returns may differ from the initial YTM because:
	- Selling the bonds *before maturity* may result in a *capital gain/loss*.
	- The cash flows may be *reinvested at a different rate* to the initial YTM.
- **Investment horizon** influences the overall gain/loss to the investor.
	- If investment horizon < Macaulay duration:
		- The effect of a *capital gain/loss* will dominate.
		- i.e., falling interest rates will lead to a higher realised return.
	- If investment horizon > Macaulay duration:
		- *Reinvestment risk* will dominate
		- i.e., falling interest rates will generate a lower realised return.

>[!info] Macaulay Duration
>Macaulay duration is a key metric used in bond investing that measures the weighted average time it takes for an investor to *recoup the bond's price through its cash flows*.
>- It is calculated by multiplying each cash flow by the time it is received, summing these values, and then dividing by the bond's price.
>$$
>\text{Macaulay Duration}, D = \frac{\sum^n_{t=1} \frac{t \times C}{(1+y)^t} + \frac{n \times M}{(1+y)^n}}{\text{Current Bond Price}}
>$$
>- $t$ : Respective time period
>- $C$ : Periodic coupon payment
>- $y$ : Periodic yield
>- $n$ : Total number of periods
>- $M$ : Maturity value

#### (2) Risk premium approach (the building block approach to fixed-income returns)
- Begins with a risk-free interest rate and adds compensation for risks required by the investor.
- Components of the required return for fixed-income asset classes:
	1. **Short-term default-free rate** $\rightarrow$ Compensation for interest rate risk
		- It is the rate on a *frequently* issued *zero-coupon government bond*, as it:
			- is of the highest quality,
			- is the most liquid security, and
			- has a maturity equal to the investment horizon.
	2. **Term premium** $\rightarrow$ Reward for duration risk
		- The default-free spot rate curve shows:
			- Expected path of short-term rates.
			- The required term premiums for each maturity.
		- Real term premiums cannot be obtained solely from the yield curve.
		- Term premiums typically:
			- are positive,
			- increase with maturity,
			- are roughly proportion to the duration, and
			- vary over time.
		- Term premium is driven by:
			1. *Inflation uncertainty*
				- High inflation implies high inflation uncertainty $\rightarrow$ increasing nominal yields $\rightarrow$ increased term premium.
			2. *Recession hedge*
				- If inflation is as a result of aggregate <mark style="background: #FFF3A3A6;">demand</mark>:
					- Nominal bond returns and growth are negatively correlation.
					- Leads to low term premiums.
				- If inflation is caused by aggregate <mark style="background: #FFF3A3A6;">supply</mark>:
					- Nominal bond returns and growth are positively correlated.
					- Leads to higher term premium.
			3. *Supply & Demand*
				- Supply of long- and short-term default-free bonds influences the <mark style="background: #FFF3A3A6;">slope of the yield curve</mark>, which affects the term premium.
			 4. *Business cycles*
				 - Business cycles influences the <mark style="background: #FFF3A3A6;">slope of the yield curve</mark>, and hence the term premium.
	3. **Credit premium** $\rightarrow$ Compensation for credit risk
		- Is the compensation for (1) *risk of default losses* and (2) *expected level of losses*.
		- The above are components of credit spreads.
		- Depends on the *credit quality*.
		- Positively related to:
			1. <mark style="background: #FFF3A3A6;">slope of the yield curve</mark>, and
			2. <mark style="background: #FFF3A3A6;">volatility of the equity market</mark>.
	4. **Liquidity premium** $\rightarrow$ Reward for illiquidity
		- Is the compensation for *holding less liquid bonds*.
		- Liquidity tends to be high for:
			1. New bonds
			2. Bonds of high quality
			3. Bonds with a simple structure
			4. Large in size bonds
			5. Bonds issued at market rates
			6. Bonds issued by a renowned frequent issuer
		- Bonds with *lower liquidity* $\rightarrow$ necessitate a *higher liquidity premium*.
		- Baseline estimate of liquidity premium = Yield spread between highest quality issuer in the market and the next highest quality large issuer.

>[!info]- Zero-coupon government bond
>- A zero-coupon government bond is a type of bond issued by a government that does not pay periodic interest payments (coupons) throughout its lifetime.
>- Instead, these bonds are sold at significant discount to their face value, and investors receive the full face value when the bond matures.

## Risks in Emerging Market Bonds
Emerging market debt involves similar risks as investing in more developed economy's debt, such as:
1. Interest rate changes,
2. Currency movements,
3. Potential for defaults, and
4. Economical and political/legal risks (less significant risks in developed markets).

### Economic Risks (Ability to Pay)
Emerging market economies are less likely able to settle their debts on-time or in-full due to:
1. Higher *wealth concentration* $\rightarrow$ only a few people own the wealth of the country.
2. Greater dependence on *cyclical industries* (e.g., commodities) and low pricing power in world markets.
3. *Restrictions* on trade, capital flows, and currency.
4. Poor *fiscal controls* and *monetary discipline*.
5. An insufficient fiscal and monetary *control system*.
6. Less educated and *inadequately skilled workforce*; poor physical *infrastructure*; lower level of *technological advancement*.
7. Dependence on *foreign borrowing*, usually in hard currencies.
8. Underdeveloped and small *financial markets*.
9. Vulnerability to *volatile capital flows*.

### Key considerations before investing in emerging markets
1. **Fiscal Deficit to GDP** - A persistent ratio above 4% should be questioned.
2. **Debt-to-GDP Ratio** - Greater than 70-80% is a sign of vulnerability for an emerging market.
3. **Annual Real Growth Rate** - Less than 4% may mean that the economy is catching up with developed economies.
4. **Current Account Deficits** - Greater than 4% of GDP may suggest a lack of competitiveness.
5. **Foreign Debt** - Greater than 50% of GDP or greater than 200% of current account receipts signals danger.
6. **Foreign Exchange Reserves** - Less than 100% of short-term debt is risky. Greater than 200% is ample.
7. **Access to external support** - Connections for support from international agencies (e.g., IMF, The World Bank).

### Political & Legal Risks / Willingness to Pay
The willingness of an emerging market to pay debt depends on a country's political and legal risks:
1. Corruption
2. Nationalisation of companies
3. Political instability
4. Weak property rights
5. Capital controls
6. Property confiscation
7. Sovereign immunity $\rightarrow$ makes it challenge to ask a sovereign borrower to settle its debts

Factors to consider:
1. Past violations of property rights.
2. Stability of the political institutions.
3. Effectiveness of the judicial system.

## Equity Forecasting
### (1) Historical Statistical Approaches
- The simplest method.
- Require collecting data in the form of past returns and using them to extrapolate future performance.
- Limitation:
	1. Equities have a *high standard deviation* relative to their mean returns.
	2. Means that historical data can often be *misleading*.
- Equities return tend to fall between 4.5% - 9% for developed countries.

![[Pasted image 20240716230827.png]]
### (2) Discounted Cash Flows (DCF) Approach
- The **Gordon growth model (constant growth model)** attempts to project growth into the future rather than simply capture what the past has delivered.
- The **Grinold-Kroner model** expands on the constant growth model.
	- Allows for adjustments from *share repurchases* and *fluctuations in overall market valuations* (price to earnings).$$
	  E(Ri) \approx D/P + (\%\Delta E - \%\Delta S) + \%\Delta P/E
	  $$
		- $E(Ri)$ : Expected equity return
		- $D/P$ : Dividend yield
		- $\%\Delta E$ : Expected percentage change in total earnings
		- $\%\Delta S$ : Expected percentage change in shares outstanding
		- $\%\Delta P/E$ : Expected percentage change in the P/E ratio
	- The equation contains a <mark style="background: #FFF3A3A6;">negative relationship to share repurchases</mark>.

### (3) Equilibrium Approach
- **Singer-Terhaar Model**
	- Combines two CAPM models:
		1. A completely *integrated market* - Each asset is priced relative to a single global market portfolio.
		2. A completely *segmented market*.
	- Each asset class in each country is *priced individually*.
$$
\text{ERP}_i = \Big[ \big(\text{Degree of integration}\big) \times \sigma_i \times \rho_{i,m} \times \frac{\text{ERP}_m}{\sigma_m} \Big] + \Big[\big(\text{Degree of segmentation} \times \sigma_i \times \frac{\text{ERP}_m}{\sigma_m}\big)\Big]
$$
		- $\text{ERP}_i$ : Equity risk premium of a partially integrated market
		- $\rho_{i, m}$ : Correlation of market with global portfolio

Explanation:
- ERP is the equity return over and above the risk-free rate.
- It is hard to forecast the equity premium.
- Analysts have to decide on the degree of integration/segmentation.
	- Equity and bond markets of *developed countries* are *highly integrated* $\rightarrow$ A range of 0.75-0.90
	- Equity and bond markets of *emerging markets* are *less integrated* $\rightarrow$ A range of 0.50-0.75
- Analysts are advised to couple forecasts with other methods of analysis.



---
## References

- [[CFA Programme - Level 3 (AnalystPrep)#Forecasting Asset Class Returns]]
- [Macaulay Duration: Definition, Formula, Example, and How It Works (investopedia.com)](https://www.investopedia.com/terms/m/macaulayduration.asp)