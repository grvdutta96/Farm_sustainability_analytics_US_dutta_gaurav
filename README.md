Proof-of-concept analytics platform demonstrating dairy sector greenhouse gas benchmarking, regional emissions intensity comparisons, and feed additive intervention ROI modelling using USDA NASS and EPA GHG Inventory data
Designed, developed, and deployed independently using publicly available agricultural data and established LCA benchmarks.
Data sources and primary focus:
• USDA NASS 2022 Census of Agriculture — state-level dairy herd sizes, average operations per region, and
regional production structure across Northeast, Midwest, South, and West U.S. production zones
• EPA Greenhouse Gas Inventory (2024) — sector-level GHG attribution for U.S. dairy: enteric fermentation
(48%), manure management (29%), and feed production (23%) as shares of cradle-to-farm-gate emissions
• Thoma et al. (2013), International Dairy Journal — national benchmark range for U.S. dairy emissions
intensity (1.00–1.45 kg CO2e/kg FPCM; national average 1.23–1.24)
• Capper et al. (2009), Journal of Animal Science — feed efficiency benchmarks (1.3–1.6 kg milk/kg DMI) for
lactating U.S. Holsteins
How key metrics are calculated:
• Emissions intensity reported in kg CO2e per kg fat-and-protein-corrected milk (FPCM), with a unit toggle to lbs
CO2e per cwt milk (conversion: ×100) for commercial dairy reporting standards
• Farm-level simulation: 45 synthetic farm points generated deterministically from state-level distributions (3 farms
per state), with bubble size scaled to total milk output and colour coded by feed efficiency quartile (high/medium/low)
• Intervention scenario modeller: enteric CH4 reduction calculated as: adoption rate × per-cow reduction × enteric
share (48%) × baseline intensity × farm milk volume (300 cows × 10,000 kg FPCM/year = 3,000,000 kg ÷ 1,000 =
3,000 MT FPCM). Carbon inset value at $20/MT CO2e. Net margin impact = (inset revenue − additive cost) ÷
total cwt milk
• MRV verification logic: farm records flagged as anomalies if intensity <0.82 or >1.65 kg CO2e/kg FPCM, feed
efficiency outside 1.28–1.72, or large herds (>2,000 cows) with implausibly high intensity (>1.40). Tier 2 verified %
= (non-flagged farms ÷ total farms) × 100; updates dynamically with region filter
• Historical trajectory: 2018–2023 USDA/EPA trend data; 2030 target (0.95 kg CO2e/kg FPCM) represents a
∼30% reduction from current baseline, consistent with industry net-zero roadmap commitments
