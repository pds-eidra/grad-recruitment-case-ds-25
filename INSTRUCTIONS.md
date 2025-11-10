# Nordic Expansion Strategy Case

You're working as a data analyst on a project for a major European retail/services company considering expansion into Sweden.

The business leaders need insights on demographic trends before they enter the market.

You are tasked with providing some analytical insights that can be useful in discussions where business leaders need to make informed decisions grounded in an understanding of the evolving demographics of Sweden. They are thinking about a wide range of things including:

- Store location strategy
- Product mix decisions
- Market sizing and timing
- Resource allocation across regions

## Data

- All of the data is provided in GeoParquet format in a geographic coordinate reference system (EPSG:4326) and rutid_inspire is a common key available across the tables.
- befolkning_1km_*.parquet: official Swedish population demographic data from Statistikmyndigheten SCB for 2015-2024 in 1km² bins according to the EU’s INSPIRE Geospatial Data initiative.
  - Available statistics
    - Total population
    - Population by age in five-year classes
    - Population by gender
  - A statistical method is used to protect individuals' data in the reported statistics. Because of this, the reported totals are not always equal to the sum of their reported parts.
- RegSO_2025_Link: Locality metadata derived from the Regionala statistikområden (RegSO) dataset for the 1km² bins.

While the data is provided in a common geospatial format, you are free to work with the data as you see fit and are not required to perform any spatial analysis to complete this case. Work to your strengths!

## Potential Analysis Directions

You can be as creative as you wish with the direction you choose to explore with this dataset. Here are some examples of questions to help give you some ideas and inspiration of the types of questions you can try to answer with this data.

1. Market Opportunity Sizing:

   - Which areas show population growth vs. decline?
   - Where are the highest-density consumer segments for different target demographics?
  
2. Location Strategy:

   - Identify clusters of target age groups (e.g., 25-45 for premium retail)
   - Urbanization trends - where are people concentrating?
   - Find areas with changing age structures (aging vs. young family influx)

3. Timing & Forecasting:

   - Project population changes to optimize entry timing
   - Identify markets reaching demographic "tipping points"
   - Assess long-term viability of different regions

## Task

- Explore the dataset and prepare some useful visualizations, predictions, insights, etc.
- Ensure that all steps are well-documented in your code.
- Don't spend more than 2-3 hours on your analysis.

## Presentation

- As part of your submission you need to prepare a visual presentation of your findings for a non-technical CEO, emphasizing actionable insights.
- The presentation should also include motivations for your choice of method.
- Highlight your findings and your approach.
- The presentation should be 15-20 minutes long, with questions and general discussion afterwards.
- Use [Marp](https://marpit.marp.app/markdown) to construct your [PRESENTATION.md](PRESENTATION.md). In VS Code you can install the [Marp for VS Code Extension](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode) to visualise your presentation in the Markdown Preview window.
- **Focus on the content and your narrative over styling.**

## Submission

**NB: Ensure you do not include large data files as part of your submission.**

1. When ready to submit, run the provided script to create your submission:
   - **Mac/Linux:** `./utils/create_submission.sh`
   - **Windows:** `.\utils\create_submission.ps1`

2. The script will ask for your full name and create `firstname_lastname.zip` with your code and analysis (excluding data files).

3. Submit the generated archive to: paul.dossantos@curamando.com
