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


## Emerging Market Equity Risks
- Characteristics of emerging markets:
	1. **Fragile economies**
	2. Political and policy **instability**
	3. **Weaker legal protections**, including weak property rights
	4. Weak **disclosure & enforcement standards**
- They are more prone to **idiosyncratic risks** where local country effects tend to be more important than global effects.
- Attention should be paid to:
	1. Accounting and disclosure standards
	2. Standards of corporate governance
	3. Property right laws
	4. Checks and balance on government actions

## Economic & Competitive Factors on Real Estate
Real estate differs from bonds and equities in that:
1. It is a *physical* asset
2. *Indivisible*
3. Heterogenous & *immobile*
4. A factor of *production* -> Directly produces returns in form of services
5. Requires *operating & maintenance costs*
6. *Illiquid*
7. *Costly to sell*
8. Property *trade infrequently*
9. *Appraisals* are used in valuing property instead of transactions

### Historical real estate returns
- Much of the usable data comes from **appraisals** rather than sales.
- Appraisal values:
	1. Smooth returns
	2. Overstate the importance of including real estate in a portfolio
	3. Understate correlations with other assets
- The time series model can be used to correct the limitations of using appraisal data.

### Real Estate Returns
The returns on the real estate market depends on the state of the economy:
--- start-multi-column: ID_c8uw
```column-settings
Number of Columns: 2
Largest Column: standard
```

Boom
- Increased demand for property.
- Property values, lease rates, and occupancy will be driven up $\rightarrow$ Stimulates construction activity.
- This leads to stronger economic activity.

--- column-break ---

Bust
- Falling demand for property.
- Over-building and over-leveraging.
- Drives property values, lease rates, and occupancy down.
- Absorbing excess supply may take a long period.
- As leases lock in tenants for longer terms and moving costs are high.

--- end-multi-column
### Capitalisation Rates
![[Pasted image 20240718213719.png|700]]
- Capitalisation rates are the standard metric for valuing real estate investments.
	- Like earnings/price ratio in equities valuation.
	- Higher Cap Rates $\rightarrow$ Lower quality, higher risk properties, in less attractive locations.
$$
\begin{align}
\text{Capitalisation Rate (Cap Rate)} & = \frac{\text{Current period net operating income}}{\text{Property value}} \\ \\
\text{Expected Return} & = \text{Cap Rate} + \text{NOI Growth Rate}
\end{align}
$$
- The long-run, **steady-state net operating income (NOI) growth rate** should be reasonably close to the *GDP growth rate* for stable periods.
- For a finite time period,
	- $E(R_{re}) = \text{Cap Rate} + \text{NOI Growth Rate} - \%\Delta\text{Cap Rate}$
- Cap Rate is used as the **discount rate** for valuing real estate property over the long term.
- Cap Rates are **positively linked to long-term interest rates**.
	- They rise in an expanding economy and fall in a recessionary economy.

### The Risk Premium Perspective on Real Estate Expected Return
- Real estate is often thought of as a hybrid asset.
- It has **bond-like characteristics**.
	- It should earn a **term premium** as it is a long-term asset.
	- Landlords have exposure to tenant credit quality, hence should earn **credit premium**.
- Similar to equities, real estate returns are **pro-cyclical**.
	- Implies the need for a strong **equity-risk premium** (relative to corporate bonds).
- Combining the bond-like characteristics with the equity characteristics mean that real estate should earn a risk premium *between bonds and stocks*.
- Liquidity:
	- Direct real estate is illiquid.
	- Investors require compensation for illiquidity.
	- Reasonable liquidity premium is **2%-4%**.

### Real Estate in Equilibrium
- After calculation of suitable risk premiums, real estate can be applied to equilibrium models (e.g., Singer-Terhaar model).
- More adjustments should be done to:
	- Eliminate the impact of smoothing from the data.
	- Add a liquidity risk premium to compensate for illiquidity.
- Direct real estate ownership is also likely to be more affected by local economic conditions than global.

### Public vs Private Real Estate
- Private Real Estate $\rightarrow$ Only large institutional investors and wealthy investors can have diversified portfolios of direct real estate investments.
- Direct property investment is costly, and diversification is difficult to achieve for small investors.
- Public Real Estate $\rightarrow$ Shares in property companies (e.g., REITs) are an alternative method of direct investment.
	- REITs have stock-like characteristics in the short run, and behave like real estate in the long run.
- Difficult to compare the investment characteristics of direct and indirect property investment due to:
	1. Return smoothing,
	2. Heterogeneity of properties, and
	3. Varying leverage.

### Long-Term Housing Returns
- Residential real estate accounts for ~75% of the total value of developed properties globally.
- It showed the best performance over the period 1870-2015 compared to equities and bonds.

## Exchange Rates Forecasting
- Asset prices are quoted in units called **currencies**.
- Change in exchange rate affects the value of assets expressed in one currency relative to another.
- Exchange rates are determined by factors affected by:
	1. Trading
	2. Regulations
	3. Customs of a country
	4. Government
	5. Financial systems

### Ways in which trade goods and services can influence exchange rates
1. **Trade Flows**
	- Effect of net trade flows on exchange rates is *relatively small*, provided that they can be financed.
	- Large trade flows relative to financing/investment flows $\rightarrow$ Is a warning sign.
2. **Purchasing Power Parity (PPP)**
	- Prices of goods and services in different countries should show changes in exchange rates.
	- Expected change in the exchange rate should be in line with expected *inflation rate differentials*.
3. **Current Account**
	- The sensitivity of exchange rates to the current account increases when restrictions are imposed on capital flows.
		- Persistent and sustained current account balances will have the biggest influence on exchange rate.
		- Pay attention to the *source of imbalance*.
	- Adjusting capital flows exerts great pressure on exchange rates.
	- Consider implications on:
		1. Capital mobility
		2. Uncovered interest rate parity
		3. Portfolio balances and composition

### Capital Mobility
Capital seeks the **highest risk-adjusted return**.
- Countries that offer better risk-adjusted returns should see capital inflows.

The expected rate of change of a foreign currency-denominated in local currency terms:
$$
E(\%\Delta S_{d/f}) = (r^d - r^f)\ +\ (\text{Term}^d - \text{Term}^f) + (\text{Credit}^d - \text{Credit}^f) + (\text{Equity}^d - \text{Equity}^f) + (\text{Liquid}^d - \text{Liquid}^f)
$$
- $E(\%\Delta S_{d/f})$ : Expected rate of change in exchange rate of domestic & foreign currency
- $r^d - r^f$ : Nominal interest rate differential of domestic & foreign markets
- $\text{Term}^d - \text{Term}^f$ : Term premium differential
- $\text{Credit}^d - \text{Credit}^f$ : Credit premium differential
- $\text{Equity}^d - \text{Equity}^f$ : Equity premium differential
- $\text{Liquid}^d - \text{Liquid}^f$ : Liquidity premium differential
- The *domestic variable* has a *positive relationship* with the expected change in currency.
- The *foreign variable* has a *negative relationship* with the expected change in currency.

### Overshooting

![[Pasted image 20240718221650.png|700]]
--- start-multi-column: ID_wo64
```column-settings
Number of Columns: 3
Largest Column: standard
```

In the short-term:
The exchange rate appreciates.

--- column-break ---

In the intermediate term:
Investors start anticipating a *reversal*, following an extended level of stronger exchange rates.

--- column-break ---

In the long-term:
Exchange rates deprecation as the investment opportunities are borne out.

--- end-multi-column
### Uncovered Interest Rate Parity (UIRP)
$$
F_0 = S_0 \times \frac{1 + i_c}{1 + i_b}
$$
- $F_0$ : Forward rate
- $S_0$ : Spot rate
- $i_c$ : Interest rate in country $c$
- $i_b$ : Interest rate in country $b$

- Asserts that the expected %-change in the exchange rate should be equal to the **nominal interest rate differential**.
	- <mark style="background: #FFF3A3A6;">Premium differentials from the previous equation do not matter</mark>.
- The *higher interest rate currency* is expected to *depreciate* to balance out the rate premium.
- **Carry trades** $\rightarrow$ Entails *borrowing in a low-interest rate currency* and converting the borrowed amount into another currency.
	- It is widely accepted that carry trades *earn meaningful profits* under most market conditions, which conflicts with UIRP.

### Hot Money

>[!info] Hot money signifies currency that quickly and regularly *moves between financial markets*, that ensures investors lock in the **highest available short-term interest rates**.

- Capital inflow from one country to another to generate **short-term interest rate difference**.
- Challenges associated with hot money:
	1. Impairs the central bank's ability to manage monetary policy.
	2. Encourage companies to borrow short-term to finance long-term needs.
	3. Exchange rate overshooting may affect non-financial businesses.
- Central banks can solve the effects of hot money flows through:
	1. Buying/selling government bonds
	2. Controlling interest rate targets
	3. Buying/selling the foreign currency

### Portfolio balance and consumption
- When a country experiences strong economic growth, its currency tends to have an increasing share in global market portfolios.
- Investors are then induced to allocate more funds to that country and currency.
	- Accompanied by the *weakening of the currency* and *increase in the risk premiums*.
- To mitigate the above effects:
	- Investors typically absorb a greater share of new assets in their home countries, known as **home currency bias**.
	- Funding growth from productivity gains with financial flows and foreign direct investments.

## Forecasting Volatility
- It is straightforward to estimate a single variance believed to be a constant.
- Estimation task is more complicated for varying variance.

### Constant variance covariance (VCV) matrix 

![[Pasted image 20240718222704.png|700]]

- Used to estimate constant variances and covariances.
- *Historical return* data is used to calculate sample variances and covariances.
- A constant CVC matrix is obtained by compiling the sample values.
--- start-multi-column: ID_31b5
```column-settings
Number of Columns: 2
Largest Column: standard
```

Advantages:
1. Sample VCV is an *unbiased estimator* of the actual VCV.
2. It is *simple*.

--- column-break ---

Disadvantages:
1. Prone to *sampling errors*.
2. Cannot be used for *large numbers* of asset classes $\rightarrow$ Some portfolios may mistakenly look riskless when the number of asset classes is more than the number of historical observations.
3. Does not consider *cross-sectional consistency*.

--- end-multi-column
#### VCV Matrices from Multi-Factor Models
- Attempts to explain the outcomes of a model using many variables simultaneously.
- Substantially reduces the number of required observations.
- Aids in achieving cross-sectional consistency.
$$
\text{Return of the i-th asset, } R_i = \alpha_i + \sum^N_{n=1}\beta_{in}F_n + \epsilon_i
$$
- $N$ : Number of common factors
- $\alpha_i$ : Intercept
- $\beta_{in}$ : $i$-th asset's sensitivity to the $n$-th factor
- $F_n$ : $n$-th factor return
- $\epsilon_i$ : Factor term unique to asset $i$ with a zero mean.

$$
\begin{align}
\text{Variance of the i-th asset, } \sigma_i^2 & = \sum^N_{p=1} \sum^N_{q=1} \beta_{ip}\beta_{iq}\rho_{pq} + V_i^2 \\ \\ 
\text{Covariance of i-th and j-th asset, } \sigma_{ij} & = \sum^N_{p=1}\sum^N_{q=1}\beta_{ip}\beta_{iq}\rho_{pq}
\end{align}
$$
- $\rho_{pq}$ : Covariance between the $p$-th and $q$-th factors
- $V_i^2$ : Variance of the $\epsilon_i$ unique factor
--- start-multi-column: ID_g6yq
```column-settings
Number of Columns: 3
Largest Column: standard
```

Assumptions for multi-factor models:
1. Factors are not redundant.
2. Factors do not have zero terms.

--- column-break ---

Roles of the assumptions:
1. Ensure meaningful matrix outcomes.
2. Avoids identifying a riskless portfolio by mistake.

--- column-break ---

Problems with multi-factor model VCV:
1. Model misspecification might lead to a more precise but less accurate VCV matrix.

--- end-multi-column
### Estimating volatility from smoothed returns

![[Pasted image 20240718223538.png|800]]

Time-Varying Volatility
- ARCH Models: Used to address **volatility clustering**.
	- Volatility clustering is characterised by periods of high and low volatilities.

## Changes in Global Investment Portfolio
### Macro-Based Recommendations
- Involve the "high-level" aspects or the broadest view possible for a portfolio.
- Looking at what is driving the *global economic growth* can help inform the process.
- Relevant questions:
	- What countries are becoming more or less competitive? Why?
	- Which stage of the business cycle are various countries in?
- These questions can help an analyst to make adjustments to:
	- Equity vs fixed income
	- Specific country investments
	- Credit ratings within fixed income portfolio
	- Currency exposure
	- Positioning on yield curve

### Trend Growth
- Higher trend growth rates would favour increasing portfolio weightings in equity and real estate.
- Outstanding bonds would be under downward pricing pressure as more fixed income with more competitive rates is issued.
- **Higher Trend Growth $\rightarrow$ Higher Real Interest Rates $\rightarrow$ Decreasing Bond Values**

### Global Integration
- The Singer-Terhaar model states that when a market becomes more globally integrated, its required return should decline.
- A decline in the required return is followed by a shift away from developed markets towards *emerging or developing markets*.

### Phases of the Business Cycle
Business cycles may vary in terms of length and intensity from country to country.
--- start-multi-column: ID_5yt4
```column-settings
Number of Columns: 2
Largest Column: standard
```

At the trough of the business cycle (before economic expansion begins):
- Increase allocations to **equity**.
- Decrease fixed-income exposures as inflation and interest rates may be ready to rise.

--- column-break ---

When the economy is at the peak, and a contraction is imminent:
- Decrease allocations to equity.
- Increase **fixed-income exposures** as inflation and interest rates may be expected to fall.

--- end-multi-column
### Monetary & Fiscal Policies
- According to the efficient market hypothesis, monetary and fiscal policy decisions <mark style="background: #FFF3A3A6;">may already be included in asset prices</mark>.
- When it is optimal to analyse policy changes?
	1. During **structural policy changes** (i.e., overhaul of the tax code)
	2. When **extreme policy decisions** are made or have not had their intended effect

### Current Account Balances
- An expanding current account deficit will often put **upward pressure** on **real required returns**. 
	- Reasoning:
		1. To *entice more savings* in the deficit country.
		2. To *attract the increased flow of capital* from abroad required to fund the deficit.

### Capital Accounts & Currencies
- Capital accounts tend to be the *main catalyst* for relative currency valuations.
- Investors will inevitably want to switch over when they perceive a higher risk-adjusted return on the portfolio of assets held in one country.
- Returns from the currency appreciation and the returns from the underlying assets should be separated. This is to decipher the cause of the returns properly.

### Quantifying the Views
General approach to quantifying views based on macro-analyses:
![[Pasted image 20240718224512.png|800]]



---
## References

- [[CFA Programme - Level 3 (AnalystPrep)#Forecasting Asset Class Returns]]
- [Macaulay Duration: Definition, Formula, Example, and How It Works (investopedia.com)](https://www.investopedia.com/terms/m/macaulayduration.asp)