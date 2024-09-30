# research-payments-ncre-2023

# Research Payments of Non-Covered Recipient Entity (NCRE) in the United States 2023

Healthcare is one of the sought-after areas on its research and development by providing healthcare workers with innovation and associated evidence. It is beneficial in developing prevention interventions, effective treatments, and care pathways. In the US, the stakeholders in the healthcare RnD include covered teaching hospitals, individual covered physicians and practitioners, and lastly non-covered recipient entity or NCREs. According to Center for Medicare and Medicaid Services (CMS), NCREs holds as the majority element of RnD in the US. Knowing what NCREs are using for research are insightful for emerging healthcare companies by answering questions such as, "Which therapeutic area has the highest records of NCREs in New York?", "Where's the most funded research in forms of medical device for Cardiology/Vascular Diseases in California?", and "What's the most-used product by NCREs in the US on the therapeutic area of neurology?" In this project, we'll answer these kinds of questions through data.

We'll use a dataset of Research Payments 2023 downloaded from [Open Payments CMS](openpaymentsdata.cms.gov) and then filtered through three conditions below:

* `Covered_Recipient_Type IS Non-Covered Recipient Entity`
* `Related_Product_Indicator IS Yes`
* `Covered_or_Noncovered_Indicator_1 IS Covered`

We will take covered NCRE records by the manufacturer company in forms of product. This segment of data will show additional info such as the products, therapeutic areas, and also total amount of research payments, all of which are essential for getting the insights.

The project consists of three sections:
* [`01-data-cleaning.ipynb`](https://nbviewer.org/github/itsalamhere/research-payments-ncre-2023/blob/main/01-data-cleaning.ipynb) - Data cleaning with Python to eliminate `ParsingError` when processing data due to different formats in several records 
* [`02-data-analysis-bigquery.ipynb`](https://nbviewer.org/github/itsalamhere/research-payments-ncre-2023/blob/main/02-data-analysis-bigquery.ipynb) - Data Analysis with BigQuery and Python by executing queries of NCREs by variables such as states, therapeutic areas, up to most-used products.
* [`03-research-payments-NCRE-2023.twb`](https://public.tableau.com/app/profile/mohamad.alamsyah/viz/research-payments-NCRE-2023/ResearchPayments2023-NCREs) - Dashboard of Research Payments with BigQuery and Tableau to look for NCRE records by state, therapeutic areas, products, and entities dynamically.

Keywords: research payments, healthcare, RnD, dashboard, BigQuery, Python, Tableau
