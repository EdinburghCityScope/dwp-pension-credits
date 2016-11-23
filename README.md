# dwp-pension-credits
Number of Pension Credit claimants in Edinburgh by age and gender.

Pension Credit (PC) were introduced on 6 October 2003 to replace the Minimum Income Guarantee (MIG). There are two parts to PC, the Guarantee Credit (GC) and the Saving Credit (SC). The GC provides financial help for people aged 60 or over whose income is below a certain level set by the law. The awarded amount will depend on other sources of income and extra amounts are added to the standard minimum for those who have: relevant housing costs; severe disabilities; or caring responsibilities. The SC is an extra amount for people aged 65 or over who have made some provision for their retirement (such as savings or a second pension) which brings their income above a level set by parliament, called the savings credit threshold. It is possible to get savings credit on top of guarantee credit.

Data shown here are derived from a 100% data source; the Work and Pensions Longitudinal Study (WPLS) which is not subject to any sampling error. The dataset provides counts of total claimants and disaggregations by age, gender, duration on benefit, partnering and some benefit specific information. The snapshots are taken at quarterly intervals at the end of February (Q1), May (Q2), August (Q3) and November (Q4). A very small number of claimants who have an unknown age or gender are included within the area total but excluded from the age and gender breakdowns as they pose a small disclosure risk. Data from the WPLS datasets are not directly comparable to the annual individual level data previously released as they were a single snapshot at a point in time and did not reflect late notifications and removals from the systems. Claim rates of GC claimants are based on the population aged 60 plus from the small area population estimates published by the National Records of Scotland.

Statistics provided by Department for Work and Pensions:  http://statistics.gov.scot/data/pension-credits

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/dwp-pension-credits.git
```

Install npm dependencies

```
cd dwp-pension-credits
npm install
```

Run the API (from the dwp-pension-credits directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
