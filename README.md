# blockcartographer.github.io

This is an embedded analytics platform for the [Loopring](https://loopring.io/#/) ecosystem and protocol. 

> <span style="font-size:larger;"> ⚠️ This resource is in limited public release and should be regarded as a work-in-progress. It is not final. </span>

### The current dashboard and its pages

1. L2 Stats
2. Deposit Graphs
3. Account Stats
4. Fees & Income
5. Risk Mgt
6. LayerSwap
7. Liquidity Pairs
8. NFT Minting
9. USD + Token Movement
10. Top Holders
11. Account List
12. Account Detail
13. Account Cumulative
14. Account Heatmap
15. Token Heatmap

### Data Sources

* https://docs.loopring.io/en/ - The official Loopring API and their doc pages.
* https://thegraph.com/hosted-service/subgraph/loopring/loopring - For comparison and validation
* https://api.santiment.net/ - A paid service provider for daily USD conversion rates for many tokens.

### Architecture

* Extract block level data from `https://api3.loopring.io/api/v3/block/getBlock?id=<block_id>`
* Extract price data from `https://api.santiment.net/graphql`
* Load to GCP Google BigQuery
* Model in dbt w/ sql & jinja-sql
* Query, aggregate and visualize in Microsoft PowerBI

![Architecture diagram](https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/81893a5a-ec4d-4316-aac5-35996ae34165_4922x3273.png)


### Modeling

`WIP`
