<div align="center">

  <h1>SR-MPE // Standard Reserve Monetary Policy Engine</h1>

  <p>An independent, non-linear system simulator built to stress-test the core monetary mechanics of <strong>Standard Reserve ($STANDARD)</strong>.</p>

  <p>
    <a href="https://standard-reserve-simulator.vercel.app"><img src="https://img.shields.io/badge/Live%20Demo-Vercel-emerald?style=flat-square" alt="Live Demo"></a>
    <a href="https://x.com/standard_rsv"><img src="https://img.shields.io/badge/Target-@standard__rsv-blue?style=flat-square" alt="Target Protocol"></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-gray?style=flat-square" alt="License"></a>
  </p>

</div>

<hr>

<h2>🎯 Core Mechanics Simulated</h2>

<p>Unlike traditional static analyses or basic text breakdowns, <strong>SR-MPE</strong> models the live algorithmic responses of the protocol’s immutable smart contracts under volatile market conditions and shifting net capital flows:</p>

<ul>
  <li><strong>Dynamic Resolution Fee Scaling ($F_{res}$):</strong> Simulates exponential fee spikes during heavy liquidity drains to neutralize malicious arbitrage exploitation.</li>
  <li><strong>Non-Linear Contraction Engine:</strong> Models automated Protocol-Owned Liquidity (POL) vault drawdowns and $STANDARD buyback & burn execution under negative net ETH flows ($F_{net} < 0$).</li>
  <li><strong>Expansion Velocity & Reserve Accrual:</strong> Calculates the logarithmic baselining of $STANDARD issuance speed during positive Uniswap v4 net capital inflows ($F_{net} > 0$).</li>
  <li><strong>Banker Branch Deflationary Pressure:</strong> Tracks total $STANDARD supply reduction resulting from mandatory license burns as Bankers scale their active branches.</li>
</ul>

<hr>

<h2>🛠️ Architecture & Math Model</h2>

<p>The simulator operates on a non-linear mathematical feedback loop to reflect actual protocol state transitions:</p>

<pre><code>               [ Uniswap v4 Net ETH Flow (F_net) ]
                                |
             +------------------+------------------+
             |                                     |
    (F_net > 0) EXPANSION                 (F_net < 0) CONTRACTION
             |                                     |
  • Logarithmic Issuance                • Dynamic Resolution Fee Hike
  • Reserve Vault Accumulation          • POL Vault Drawdown
  • License Burn Deflation              • Automated Buyback & Burn
</code></pre>

<hr>

<h2>🚀 Quick Start & Deployment</h2>

<p>Since the engine is built as a lightweight, single-file interactive Web3 dashboard, no local Node.js environment or build step is required.</p>

<ol>
  <li>Clone the repository:
    <pre><code>git clone https://github.com/YOUR_USERNAME/standard-reserve-simulator.git</code></pre>
  </li>
  <li>Open <code>index.html</code> directly in any modern browser, or deploy directly to <strong>Vercel / Netlify</strong> with a single click.</li>
</ol>

<hr>

<h2>📜 Disclaimer</h2>

<p>This project is an independent community-built research and simulation tool created for the <strong>Standard Reserve ($STANDARD)</strong> ecosystem. It is not official financial advice and serves exclusively as a mechanism testbed.</p>
