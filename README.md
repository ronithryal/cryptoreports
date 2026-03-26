# cryptoreports
Repo where I host all my crypto research and analysis. **NOT FINANCIAL ADVICE**
---

## Liquidity Duration on Morpho Blue (Ethereum) - Mar 26, 2026
**Beyond TVL: 117 Weeks of On-Chain Evidence on Morpho’s Liquidity Duration**

TVL is a snapshot. It tells you how much is deposited today, not how long that capital actually sticks around.

I ran three reproducible on-chain queries on Morpho Blue (Ethereum) to measure capital *duration* and flow behavior, not just TVL.

📊 **What the data shows**
- **$225.9B** in cumulative USDC supply-event volume **(gross inflows, Jan ’24–Mar ’26)** carries a USD-weighted average deposit age of **192.6 days**. 
- Early depositor cohorts (Jan–Jun ’24) exhibit **35–45% 90‑day re‑engagement**, versus roughly **~10%** for later cohorts. 
- **32.5%** of weeks (38 of 117) show **organic inflows** — net USDC inflows even as prevailing borrow rates decline week‑over‑week. 

🔬 **How it was measured**
- Looked through MetaMorpho vaults by attributing deposits to underlying `owner` addresses, reducing the vault “Passenger Problem.” 
- Normalized every supply event by token decimals and contemporaneous USD prices. 
- Classified weekly net USDC flows against on-chain borrow‑rate changes to distinguish organic vs. rate‑chasing weeks. 

💡 **Why it matters**
The evidence is **consistent with** a subset of Morpho Blue liquidity behaving like longer‑horizon, relatively rate‑insensitive capital rather than purely short‑term yield‑chasing deposits. For DeFi treasury and risk teams, understanding duration and flow behavior is a prerequisite for treating any protocol as credit infrastructure rather than a trading venue. 

This report is Ethereum‑only and exploratory, but all queries are public and fully reproducible. Follow‑up work will benchmark these metrics against Aave/Spark and extend the framework cross‑chain. 

🔗 **https://github.com/ronithryal/cryptoreports/blob/main/Liquidity%20Duration%20on%20Morpho%20Blue%20(Ethereum).pdf**  
Dune queries: **6871840**, **6872058**, **6872073**  

#DeFi #CreditMarkets #MorphoBlue #InstitutionalDeFi #OnChainResearch

---

## License

Code (notebooks, scripts, and utilities) in this repository is licensed under the MIT License.

The written research reports and associated figures are intended for open research use. If you use or reference this report in your own work, please cite it as:

Yalamanchili, Ronith. **“[Title of report]”** [date published].
