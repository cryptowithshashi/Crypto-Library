# AMM (Automated Market Maker) Architecture

AMMs are algorithmic trading protocols that enable decentralized token swaps using mathematical invariants like constant product (x*y=k) and concentrated liquidity mechanisms.

## Resources

### Uniswap

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Uniswap V3 Core Documentation](https://docs.uniswap.org/contracts/v3/overview) | Uniswap Labs | (Spec; 2021) Essential concentrated liquidity protocol implementation and smart contract reference. [License: MIT] |
| [Uniswap V3 Whitepaper](https://app.uniswap.org/whitepaper-v3.pdf) | Uniswap Labs | (Whitepaper; 2021) Mathematical foundations of concentrated liquidity and tick-based AMM design. |
| [Uniswap V3 Python SDK](https://uniswap-v3.readthedocs.io/en/latest/uniswap.v3.html) | Community | (SDK; 2024) Python library for Uniswap V3 interactions with pool math. [License: MIT] |



### Curve Finance

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [StableSwap Efficient Mechanism for Stablecoin Liquidity](https://curve.fi/files/stableswap-paper.pdf) | Curve Finance | (Whitepaper; 2019) Hybrid constant product/constant sum invariant for minimal stablecoin slippage. |
| [Curve Technical Documentation](https://docs.curve.finance/stableswap-exchange/overview/) | Curve Finance | (Spec; 2023) StableSwap invariant implementation details and pool mechanics documentation. [License: MIT] |
| [Understanding StableSwap (Curve)](https://miguelmota.com/blog/understanding-stableswap-curve/) | Miguel Mota | (Tutorial; 2024) Mathematical derivation and practical examples of Curve's StableSwap algorithm. |
| [Understanding the Curve AMM StableSwap Invariant](https://atulagarwal.dev/posts/curveamm/stableswap/) | Atul Agarwal | (Tutorial; 2022) Deep mathematical analysis of StableSwap invariant with worked examples. |
| [Curve V1 StableSwap Invariant Analysis](https://medium.com/@0xmirai77/curve-v1-the-stableswap-invariant-f87ad7641aa0) | 0xmirai77 | (Research; 2023) Technical breakdown of StableSwap transition between constant sum/product. |
| [Curve Slippage Analysis](https://pandichef.medium.com/the-slippage-ratio-a-new-metric-to-understand-curve-fis-amm-protocol-fddf0ba4d6c8) | Pandichef | (Research; 2024) Quantitative analysis of slippage ratios in Curve pools. |


### Balancer

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Balancer Weighted Pools](https://docs.balancer.fi/concepts/explore-available-balancer-pools/weighted-pool/weighted-pool.html) | Balancer Labs | (Spec; 2024) Generalized AMM with arbitrary token weights and multi-asset pools. [License: GPL-3.0] |
| [Balancer Impermanent Loss Analysis](https://threesigma.xyz/blog/amm/balancer-impermanent-loss-lp-guide) | Three Sigma | (Research; 2024) Comprehensive impermanent loss formulas and calculations for weighted pools. |
| [Balancer Impermanent Loss Calculator](https://baller.netlify.app/) | Baller | (Tool; 2024) Interactive simulator for IL calculations across different pool weights. [License: Open Source] |

## Recommended books & essential reads

### AMM & DeFi Overviews

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Automated Market Makers: A Practical Guide to Decentralized Exchanges and Cryptocurrency Trading](https://annas-archive.org/slow_download/53f5790cfd1bbab5776e562b731df132/0/2) | N/A | Practical, AMM-focused book covering Uniswap, Curve, Balancer and worked examples; good for protocol-level intuition and code pointers. |
| [DeFi and the Future of Finance](https://annas-archive.org/md5/5d3de50eaa5b6bdde688103459308e99) | N/A | Concise industry overview that explains DeFi primitives (including AMMs) and practical risk/governance considerations; great starting high-level read. |

---

### Token Design & Tokenomics

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Token Economy](https://annas-archive.org/md5/66f127120561294d18abec12e8ad1e22) | N/A | Rigorous treatment of token design, incentives and governance; helps understand why AMM parameters and fee models matter to tokenomics. |

---

### Smart Contract & Blockchain Engineering

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Mastering Ethereum](https://annas-archive.org/md5/81572c7e01c91ab833c132dfebe5449a) | Antonopoulos & Wood | Hands-on Ethereum dev book: smart-contract patterns, security, testing and how contracts interact with off-chain tooling. |

---

### Market Microstructure & Execution

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Market Microstructure Theory](https://annas-archive.org/md5/60973c35892845b0ae3ef5dd8a6e66c4) | Maureen O’Hara | The canonical textbook on price impact, liquidity, and trade execution; provides the academic foundations for thinking about slippage and liquidity provision. |
| [High-Frequency Trading: A Practical Guide](https://annas-archive.org/md5/ba5a95225f922ea47a236b5a9d3950ea) | Irene Aldridge | Useful for understanding market impact, latency, and MEV parallels. |
| [Algorithmic Trading and DMA](https://annas-archive.org/md5/e8a3f780fb7625a2dcf1632825936fb7) | Barry Johnson | Practical reference on execution algorithms and order routing mechanics (helps translate order-book intuition into AMM impact thinking). |

## Tutorials & Walkthroughs

- [Curve V1 AMM Equation Explained](https://youtu.be/oUqFeJPnq3s?si=pLu88R2Lu7-vWAnq)
- [Pegged and Stablecoin AMM](https://youtu.be/_UfsarYm6f8?si=soEH-v-qOgE9wMZy)
- [What is Curve Finance in Crypto? (Animated Explanation)](https://youtu.be/37pEOqDOvGQ?si=tLb8QzN6tK2YDMyi)
- [Curve - Math | DeFi](https://youtu.be/GuD3jkPgPgU?si=s6wPlZY1Lx3pKt1c)

## 

- [The Slippage Ratio: A New Metric to Understand Curve.fi's AMM Protocol" by Panda Chef for the original framework.](https://pandichef.medium.com/the-slippage-ratio-a-new-metric-to-understand-curve-fis-amm-protocol-fddf0ba4d6c8)
- [A derivation of Curve’s Stable Swap price and slippage: by Arthur Bagourd for the rigorous mathematical breakdown.](https://www.arthur.bagourd.com/wp-content/uploads/2022/10/stableswapexplainer.pdf)
- [Understanding StableSwap (Curve)" by Miguel Mota.](https://miguelmota.com/blog/understanding-stableswap-curve/)
- Curve Slippage Analysis - Quantitative framework for analyzing slippage ratios in StableSwap pools, introducing the slippage ratio metric for pool efficiency evaluation.
- Balancer Impermanent Loss Analysis - Mathematical analysis of IL in weighted pools, demonstrating how token weights affect loss magnitudes across different scenarios.
- Curve V1 StableSwap Invariant Analysis - Technical breakdown of the mathematical properties enabling StableSwap's efficiency for stablecoin trading.

## Datasets & Queries
*Dune Analytics* - AMM analytics dashboards with:

- Daily/weekly volume and liquidity metrics
- Impermanent loss tracking across protocols
Fee collection and LP returns analysis
MEV impact measurements

*BigQuery Public Datasets* - Ethereum blockchain data for:

- Historical AMM trade analysis
- Slippage distribution studies
- Liquidity provider behavior patterns

## License & Disclaimer
This resource is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). Content is for educational and informational purposes only. Always consult qualified legal counsel for specific compliance requirements.

Regulatory requirements change frequently. Verify current requirements with appropriate authorities. Contributors are not responsible for the accuracy, completeness, or currency of external resources.

- Last Updated: August 27, 2025 
- Maintainer: cryptowithshashisupport@gmail.com 
- Contributors: 0
