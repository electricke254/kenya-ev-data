🇰🇪 Kenya EV Data

Open data on electric vehicle adoption, charging infrastructure, and sustainable mobility in Kenya.

Maintained by Electric Kenya — Kenya's electric vehicle intelligence platform — and Tech-ish Kenya.
⸻
About This Repository

Kenya generates approximately 90% of its electricity from renewable sources — geothermal, hydro, wind, and solar — making it one of the cleanest grids on Earth for EV charging. Yet the data needed to track, analyse, and accelerate EV adoption in the country has been scattered, inconsistent, and hard to access.

This repository provides open, structured data on:

- EV Charging Stations across all 47 counties in Kenya — locations, operators, connector types, power output, pricing, and status
- Electric Vehicles available in or relevant to the Kenyan market — specifications, range, pricing context
- Policy & Regulation summaries affecting EV adoption — import duties, excise rates, standards

All data is sourced, verified, and maintained by the Electric Kenya editorial and research team.

Data Files
File	Description	Format	Last Updated
data/charging-stations-kenya.csv	EV charging stations across Kenya with location, operator, power, connectors, pricing, status	CSV	April 2026
data/ev-models-kenya.csv	Electric and hybrid vehicles tracked for the Kenyan market	CSV	April 2026
data/ev-import-duty-rates.csv	Current import duty, excise, and tax rates for EV vs ICE vehicles in Kenya	CSV	April 2026
llms.txt	LLM-friendly site description for electric.ke following the llms.txt specification	Markdown	April 2026

Interactive Tools

These datasets power the following tools on electric.ke:

- Charging Station Map — Interactive map with filtering by county, connector type, charging speed, and operator status across all 47 counties
- Vehicle Database — Browse and compare EV specs side by side with colour-coded strengths and weaknesses
- Import Duty Calculator — Calculate the full landed cost of importing an EV to Kenya (CIF, duties, excise, VAT, levies) with live exchange rates

Key Context

Why Kenya Matters for EVs

- ~90% renewable electricity grid — EVs charged here run on geothermal, hydro, wind, and solar
- 10% excise duty for EVs vs 25% for ICE vehicles under the Finance Act 2023
- M-PESA infrastructure enables pay-as-you-go EV financing and mobile charging payments
- Growing local manufacturing — Roam builds electric motorcycles domestically
- Active startup ecosystem — BasiGo (electric buses), MojaEV (electric taxis), Roam (electric motorcycles), ChargeNet, EvChaja

Recent Developments

- Kenya raised $1.2 billion through a historic green bond (March 2026)
- I&M Bank sealed a $30 million green finance facility with Sweden's Sida for clean energy and transport lending
- Analysis: How cheap nuclear electricity could transform EV charging economics
- Analysis: Why Kenya needs both nuclear and solar
- Four climate ventures received $273k in funding from BFA Global and FSD Africa

Data Schema

Charging Stations (charging-stations-kenya.csv)
Column	Type	Description
station_name	string	Name of the charging station
operator	string	Company operating the station
county	string	Kenyan county where the station is located
location_detail	string	Specific address or landmark
latitude	float	GPS latitude
longitude	float	GPS longitude
power_kw	float	Maximum charging power in kilowatts
connector_types	string	Comma-separated connector types (CCS2, CHAdeMO, Type 2, etc.)
num_connectors	integer	Number of charging connectors available
price_per_kwh_kes	string	Price in KES per kWh (if available)
status	string	Operational, Under Construction, Planned, Out of Service
source_url	string	Link to station details on electric.ke

EV Models (ev-models-kenya.csv)
Column	Type	Description
make	string	Vehicle manufacturer
model	string	Vehicle model name
variant	string	Specific variant (e.g., AWD, EREV)
type	string	Electric, Hybrid (HEV), Plug-in Hybrid (PHEV)
range_km	integer	WLTP/CLTC range in kilometres
power_kw	integer	Maximum power output in kilowatts
acceleration_0_100	float	0-100 km/h time in seconds (if available)
source_url	string	Link to vehicle details on electric.ke

Usage

This data is free to use for research, journalism, policy analysis, application development, and educational purposes. If you use this data, please credit:

Data source: Electric Kenya (https://electric.ke)
Repository: https://github.com/electricke254/kenya-ev-data


Contributing

We welcome contributions — particularly:

- Corrections to charging station data (new stations, status changes, pricing updates)
- Additional vehicle models entering the Kenyan market
- Policy or regulatory updates affecting EV adoption
- Translations (Swahili, other Kenyan languages)

Please open an issue or submit a pull request.

Related Resources

- Electric Kenya — Kenya's EV intelligence platform
- Tech-ish Kenya — Kenya's largest independent technology news platform
- E-Mobility Association of Kenya — Industry body for electric mobility
- KEBS Electric Vehicle Standards — Kenya Bureau of Standards EV regulations
- Kenya's NDC Transport Targets — Nationally Determined Contribution for transport emissions

Contact

- Website: electric.ke
- X/Twitter: @Electric_254
- Telegram: Electric Kenya
- Email: Contact form

Licence

This data is released under the Creative Commons Attribution 4.0 International (CC BY 4.0) licence. You are free to share and adapt this data for any purpose, provided you give appropriate credit.
⸻
Built and maintained by Electric Kenya · Powered by Tech-ish Kenya
