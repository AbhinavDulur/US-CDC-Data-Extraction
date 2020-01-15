# US-CDC-Data-Extraction
The objective of this file is to obtain information smoking information about a particular State by using the U.S. CDC Data API's. The end goal is to enter a State and retrieve associated smoking information.

- API Usage Tutorial:
https://dev.socrata.com/foundry/chronicdata.cdc.gov/wsas-xwh5

- U.S. CDC Data:
https://chronicdata.cdc.gov/Survey-Data/Behavioral-Risk-Factor-Data-Tobacco-Use-2011-to-pr/wsas-xwh5

- Variables Description and Methodology
https://chronicdata.cdc.gov/Survey-Data/Behavior-Risk-Factor-Surveillance-System-BRFSS-Glo/5amh-5sx3


We will use the Behavioral Risk Factor Data: Tobacco Use (2011 to present). The following is a brief description from their website:

*The BRFSS is a continuous, state-based surveillance system that collects information about modifiable risk factors for chronic diseases and other leading causes of death. The data for the STATE System were extracted from the annual BRFSS surveys from participating states. Tobacco topics included are cigarette and e-cigarette use prevalence by demographics, cigarette and e-cigarette use frequency, and quit attempts.*

*For 2011 data and forward, a random-digit dialing system was used to select samples of adults in households with landline or cellular telephones. The sample represented adults from each state who were civilian, aged 18 years or older and not institutionalized.*

Using the "Socrata Query Language" we can specify what we want from the data. For now, I will specify that I want the following:
- Year = 2018, as this is the most recent year in the dataset

- Topic Description = Cigarette Use (Adults), as we want to look at Cigarette use within adults

- age = All Ages

- Gender = Overall

- Race = All Races

- Education - All Grades

- Measure Description = Current Smoking
    - This is defined as: Persons who reported ever smoking at least 100 cigarettes and who currently smoke every day or on some days. Respondents who answered "don't know" or who refused to answer were excluded from the analysis, as were respondents with missing current smoking information.
