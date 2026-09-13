# RippleEffect_Project
What happens when the countries feeding the world stop selling

Ripple Effect: What Happens When the Countries Feeding the World Stop Selling

A study of Rice and Wheat export restrictions, 2007 to 2025. Built for the Women in Data "What's Cooking?" Datathon 2026.

What this project asks

When a country supplying a large share of the world's rice or wheat stops selling, what actually happens? Does it hurt the countries most dependent on that seller the most, or does the shock spread further, and deeper, than that?

This project tests it using real data from UN Comtrade, the World Bank, FAOSTAT, and the OECD, tracing the effect from the countries buying, to the countries selling, to the farmers growing the crop.

Live tool

[Link to be added once GitHub Pages is live]

Open index.html directly, or visit the live link above, for the interactive trade map, diversification filter, and shock calculator.

Repository structure
├── index.html                                      the live tool
├── Ripple_Effect_Analysis.ipynb                    full analysis: restriction data cleaning, export-side signal testing, food security trend
├── Pass_Through_All_Groups.ipynb                   the pass-through rate, tested for importers, exporters, all countries, and farmers
├── Dependency_vs_Global_Shock.ipynb                tests whether dependency predicts price impact
├── Diversification_Analysis.ipynb                  tests whether supplier count predicts availability
└── data/
    ├── oecd-database-on-export-restrictions-for-staple-crops-2025.xlsx
    ├── events_clean_final.csv
    ├── Importers_rice2002-2013.csv
    ├── Importers_rice2014-2025.csv
    ├── Importers_wheat2002-2013.csv
    ├── Importers_wheat2014-2025.csv
    ├── Comtrade_2013-2002.csv
    ├── Comtrade_2014-2025.csv
    ├── comtrade_2002-2023_wheat.csv
    ├── comtrade_2014-2025_wheat.csv
    ├── CMO-Historical-Data-Annual.xlsx
    ├── Trade_CropsLivestock_E_All_Data.csv
    ├── Prices_E_All_Data.csv
    ├── FAOSTAT_comsumerpriceindices.csv
    └── Food_Security_Data_E_All_Data.csv
Key findings

Dependency does not predict price impact. Tested four separate ways, across a 50-observation panel, no relationship.

The pass-through rate is real, and it holds at every level tested:

	Top importers	Exporters	All countries	Farmers
Rice	0.50%	0.61%	0.33%	0.34%
Wheat	0.93%	0.70%	0.65%	0.57%

For every 1% the world price rises, this is how much a typical country's own price rises, at that level of the supply chain.

Supplier diversification, not dependency, predicts real shortage risk. Confirmed in two separate crises, Vietnam's 2020 rice ban and Russia's 2022 wheat disruption. Only two countries currently sit in the highest-risk zone, Philippines (Rice) and Türkiye (Wheat), both with just 2 real suppliers.

Team

SheServes- Akshata, Nina, Kasturi, Sayuja

Data sources

OECD-AMIS Export Restrictions Database, UN Comtrade, World Bank Commodity Markets Outlook, FAOSTAT (Trade, Prices, Consumer Price Indices, and Food Security and Nutrition domains)
