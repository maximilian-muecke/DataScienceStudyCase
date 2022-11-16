# Data Science Case Study: Supplier Audit Results Prediction
Data Science Case Study November 2022 / Think Tank

**Context**: Imagine you are a Data Scientist in the Supply Chain Delivery Assurance Department of BMW Group and you are responsible for predicting the supplier audit results to support business decisions. Before and during new production of model cars, supplier audits are conducted by audit experts and it is an important process to ensure the production quality. The audit experts want to have data points where they can see the qualification of certain suppliers in the future.

**Supplier Audit Process**: T1, T2, T3 represent the different stages of the production, and the result corresponds to the most recent stage.

Colors are used by the audit experts to easily show the qualification of a supplier:

> **Green** indicates that the suppliers are qualified in the current audit process.
> **Yellow** means that they receive warnings.
> **Red** means that the suppliers are disqualified.

## Datasets
Two datasets are available for this case study:

- **Audit History: Dataset of supplier audit histories.**

		* SupplierId: The supplier who is involved in the audit process.
		* RecentMonth: Update of result for the month (e.g, see table below).
		* RecentTimeStamp: The time when the audit is conducted.
		* DerivativeName: The type of model car the supplier is supplying for, one supplier can supply for different model cars.
		* DerivativeRegion: The region where the derivative is in production.
		* ProductionLine: The name code of the production line.
		* T1Color: The color shows the qualification of the supplier if they are in stage T1.
		* T2Color: The color shows the qualification of the supplier if they are in stage T2.
		* T3Color: The color shows the qualification of the supplier if they are in stage T3.
		* Result: The color of the current result.

|Derivative Name|Recent Month|T1 Color|T2 Color|T3 Color|Result|
|:-:|:-:|:-:|:-:|:-:|:-:|
|D1|Jun 2022|Green|Green|Green|Green|
|D1|May 2022|Green|Yellow|Red|Red|
|D1|Apr 2022|Green|Yellow|-|Yellow|
|D1|Mar 2022|Green|Red|-|Red|
|D1|Feb 2022|Green|-|-|Green|
|D1|Jan 2022|Green|-|-|Green|

- **Supplier Performance KPIs: Dataset for key supplier performance indicators.**

		* SupplierId: The supplier who has records of wrong deliveries, weekly reds, backlogs or LPKM score.
	
		* Amount_WD_3M, Amount_WD_6M, Amount_WD_12M: Wrong deliveries happen when suppliers send wrong material parts. These features are the amount of wrong deliveries in the last 3 months, 6 months or 12 months for each supplier.


		* Amount_Backlogs_3M, Amount_Backlogs_6M, Amount_Backlogs_12M: Backlogs happen when suppliers cannot deliver parts on time. These features are the amount of backlogs in the last 3 months, 6 months or 12 months for each supplier.


		* 12_Month_LPKM: LPKM score is the grade of the supplier regarding the KPIs for the last 12 months (the higher the better).


		* BadSupplierIndicator: Indicator of whether the supplier has bad performance before.

## Leading Points

1. Explore the datasets, if necessary clean them and keep and / or create relevant features.
2.  Analyze the features, what statements can you make?
3. Train a prediction model to predict the result (green, yellow or red) of the audit process. How good is your model performance? How would you tweak it?
4. Given the results of the analysis and prediction, how would you explain them to the audit experts? What advice would you give to the business?

*Optional: You can also implement / explain a Causal Machine Learning approach (e.g. python libraries: DoWHY, DECI, PyWHY) to increase the model explainability.*

# Enjoy the task and blow our minds !
