<svg width="800" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@500&amp;display=swap');
    
    .text-base {
      font-family: 'Fira Code', monospace;
      fill: #FFFFFF;
    }
    
    .text-orange {
      fill: #F7931A;
    }
    
    /* Code typing animation effect */
    @keyframes type {
      from { width: 0; }
      to { width: 100%; }
    }
    
    .code-line {
      overflow: hidden;
      white-space: nowrap;
      animation: type 2s steps(40, end);
    }

    /* Floating/Popping Sat coins */
    @keyframes popSat {
      0% {
        transform: translate(0, 0) scale(1);
        opacity: 0;
      }
      20% {
        opacity: 1;
        transform: translate(0, -20px) scale(1.2);
      }
      100% {
        transform: translate(10px, -80px) scale(0.8);
        opacity: 0;
      }
    }

    .sat-coin {
      animation: popSat 3s ease-out infinite;
      opacity: 0;
    }

    /* Staggered animation for popping coins */
    #sat1 { animation-delay: 0.2s; }
    #sat2 { animation-delay: 1.5s; }
    #sat3 { animation-delay: 0.8s; }
    #sat4 { animation-delay: 2.2s; }
  </style>

  <rect width="100%" height="100%" fill="#1A1A1A" rx="10"/>

  <g transform="translate(30, 40)">
    <text x="0" y="0" class="text-base text-orange" font-size="20">root@Africa:~$ ./SpendSat_Init</text>
    <g class="code-line">
      <text x="0" y="30" class="text-base" font-size="16">> Trust Layer: [OK]</text>
    </g>
    <g class="code-line">
      <text x="0" y="55" class="text-base" font-size="16">> Citrusrate API: [OK]</text>
    </g>
    <g class="code-line">
      <text x="0" y="80" class="text-base text-orange" font-size="16">> OrangePillar: VERIFIED</text>
    </g>
    <g class="code-line">
      <text x="0" y="110" class="text-base" font-size="16">> > Status: Bridging Trust Gap...</text>
    </g>
  </g>
  
  <g transform="translate(600, 100)">
    <path d="M-40,0 L0,-40 L40,0 L0,40 Z" fill="#F7931A" opacity="0.8"/>
    <text x="-15" y="5" class="text-base" font-size="24" font-weight="bold">⚡</text>
    
    <g class="sat-coin" id="sat1" transform="translate(-50, -10)">
      <circle cx="0" cy="0" r="10" fill="#FFFFFF" stroke="#F7931A" stroke-width="2"/>
      <text x="-4" y="4" font-family="Arial" font-size="12" fill="#F7931A">₿</text>
    </g>
    <g class="sat-coin" id="sat2" transform="translate(40, -30)">
      <circle cx="0" cy="0" r="8" fill="#F7931A"/>
      <text x="-3" y="3" font-family="Arial" font-size="10" fill="#FFFFFF">s</text>
    </g>
    <g class="sat-coin" id="sat3" transform="translate(-20, -50)">
      <circle cx="0" cy="0" r="10" fill="#FFFFFF" stroke="#F7931A" stroke-width="2"/>
      <text x="-4" y="4" font-family="Arial" font-size="12" fill="#F7931A">₿</text>
    </g>
    <g class="sat-coin" id="sat4" transform="translate(60, -60)">
      <circle cx="0" cy="0" r="9" fill="#F7931A"/>
      <text x="-3" y="3" font-family="Arial" font-size="11" fill="#FFFFFF">s</text>
    </g>
  </g>
</svg>

# SpendSat-Bitcoin-Trust-Spending-Infrastructure

<p align="center">
  <img src="./spendsat-header.svg" width="100%" alt="SpendSat Core Infrastructure Initialize">
</p>

## ⚡ project_manifest: Bridging the trust gap for Bitcoin commerce in Africa.

![Bitcoin Badge](https://img.shields.io/badge/Network-Bitcoin-orange?style=flat-square) ![Lightning Badge](https://img.shields.io/badge/Layer-Lightning-yellow?style=flat-square) ![Role](https://img.shields.io/badge/Role-Lead%20Product%20Manager-white?style=flat-square)

### 🎯 /vision/
Enabling hyper-local Bitcoin circular economies in emerging markets. **SpendSat** isn't just a payment gateway; it's the reputation layer that allows spenders and merchants to transact with total confidence.

---

### 🛑 the_problem.log
Despite high adoption rates, Bitcoin is rarely used for daily commerce in Africa due to three major constraints:
* **[VOLATILITY_ANXIETY]:** Merchants struggle to price goods in a fluctuating asset.
* **[TRUST_DEFICIT]:** Spenders are hesitant to send non-reversible transactions to informal or unverified merchants.
* **[DISCOVERY_GAP]:** No unified directory for Lightning-ready businesses.

### 💡 the_solution (PM Strategy)
I spearheaded the development of a non-custodial marketplace infrastructure powered by the **Citrusrate.com API**, structured around three distinct modules:

#### 🟠 /core_pillars/
1.  **merchants:** Frictionless onboarding with real-time fiat-to-sats conversion to hedge against volatility.
2.  **spenders:** A location-aware discovery engine for instant, low-fee Lightning payments.
3.  **orange_pillars:** A decentralized verification layer where trusted community members vouch for merchant quality, creating a "Web of Trust."



---

### 🛠 deliverables/
As the Lead PM, I managed the end-to-end product lifecycle. View the infrastructure blueprints:

| Artifact | Description | Link |
| :--- | :--- | :--- |
| **Product Requirement Document** | System specs, user stories, and technical constraints. | [📄 /PRD/README.md](./PRD/README.md) |
| **User Journey Mapping** | Visualization of the Spender vs. Merchant experience. | [🗺️ /UX-Flows/user-flow.png](./UX-Flows/user-flow.png) |
| **Sprint Management** | Kanban boards and velocity tracking for the MVP phase. | [🚀 /Roadmap/sprint-1.md](./Roadmap/sprint-1.md) |

---

### 📈 key_metrics_tracked/
* `merchant_survival_rate_90d`: Retention of active merchants.
* `repeat_spender_ratio`: Measuring true cyclical usage vs. one-off trading.
* `iou_repayment_integrity`: Orange Pillar accuracy scores.

---

### 🎨 interface_aesthetics/
* `color_primary`: `#F7931A` (Bitcoin Orange)
* `color_secondary`: `#FFFFFF` (White)
* `color_accent`: `#1A1A1A` (Terminal Black)
