# Advanced Recycling & Macroeconomic Competitiveness: A Theoretical Model
**Master's Thesis — MSc in Economics and Policy for Global Sustainability**
*Sapienza, University of Rome | 110/110 Summa Cum Laude | A.Y. 2024–2025*

## Research Question
In the context of the transition to a circular economy, advanced recycling is often associated with significant economic barriers related to technological costs. Can these costs be offset by reduced dependency on virgin critical raw materials (CRMs) and lower fiscal burdens from emissions ? Can this transition generate sustainable economic growth?

## Motivation
The energy transition is creating an unprecedented demand shock for critical raw materials. According to the IEA, demand for CRMs such as lithium, cobalt and nickel is projected to increase by up to 450% by 2050 relative to 2018 levels. At the same time, materials now account for up to 70% of total battery costs, and supply remains structurally inelastic due to:

*   **Declining ore quality:** Extraction requires increasing energy and generates more waste per unit of output.
*   **Long lead times:** Over 16 years to bring a new mine to production.
*   **Geographical oligopoly:** China, Australia, DRC, Indonesia and Peru control the majority of global supply.

Conventional recycling techniques (mechanical, pyrometallurgical) are inadequate: they are energy-intensive, polluting, and lead to downcycling — material quality loss that prevents true closed-loop recovery. Advanced recycling technologies (hydrometallurgy, direct recycling, bioleaching) can recover CRMs at battery-grade purity (>95%), but face steep initial cost curves.

The EU has responded with the Critical Raw Materials Act (CRMA), targeting 25% of strategic consumption from recycled sources by 2030. This thesis models the macroeconomic conditions under which this transition becomes viable.

## Model Structure (Chapter 4)
The model considers a representative firm producing a final output (e.g., batteries) subject to a negative environmental feedback loop.

**Production with Environmental Damage**
$$Y_t = A e^{-Z_t} M_t$$
Output $Y_t$ depends on a productivity factor $A$, a material input aggregate $M_t$, and an environmental damage term $e^{-Z_t}$. Pollution accumulated in stock $Z_t$ reduces total factor productivity — the environmental cost of today's production is borne in future periods.

**Pollution Accumulation**
$$Z_{t+1} = (1 - \delta_Z) Z_t + E_t, \quad \delta_Z \in (0,1)$$
Pollution stock is persistent: emissions $E_t$ accumulate and only partially decay at rate $\delta_Z$. This captures a key real-world feature — environmental degradation does not self-correct instantaneously.

**CES Input Aggregator**
$$M_t = \left[ w R_t^\rho + (1-w) (A_V V_t)^\rho \right]^{\frac{1}{\rho}}, \quad \rho = \frac{\sigma-1}{\sigma}$$
The material input $M_t$ is a CES (Constant Elasticity of Substitution) aggregate of:
*   $R_t$ — virgin raw material (extraction)
*   $V_t$ — recycled input
*   $A_V$ — technological efficiency parameter for recycling (advances in $A_V$ reflect R&D progress)
*   $\sigma$ — elasticity of substitution between virgin and recycled material

Imperfect substitutability captures the real constraint that recycled materials cannot always replace virgin inputs directly, but improved technology raises $A_V$ and reduces this gap.

**Convex Costs**
Both input sources carry convex (quadratic) costs, reflecting real structural constraints:
*   **Virgin material:** $a_R R_t^2$ — convexity reflects supply inelasticity (declining ore quality, geopolitical risk, oligopoly).
*   **Recycled material:** $b V_t^2$ — convexity reflects initial technological barriers (infrastructure, scale-up costs).

**Abatement Decision**
The firm also chooses a mitigation rate $u_t \in [0,1]$. Higher abatement reduces emissions (lowering future damage and tax burden) but entails increasing marginal costs per unit of output. This introduces a double trade-off: input mix choice and abatement intensity.

## Key Results

### Market Failure Baseline
Without policy intervention, the firm behaves myopically: it does not internalise the future productivity cost of current pollution. The equilibrium is distorted toward:
*   Maximum virgin resource extraction
*   Minimum recycled input use
*   Insufficient abatement

The recycling cost curve remains too steep relative to extraction costs; the firm rationally chooses extraction. This constitutes a market failure with social welfare below the optimum.

### First-Best Policy Mix
The model identifies two complementary policy levers required to reach the social optimum:

1.  **Environmental Taxation:** A tax on emissions raises the effective cost of pollution, inducing higher abatement $u_t$ and reducing virgin extraction. However, the model highlights a critical risk: if the tax rate increases without sufficient technological alternatives, the firm cannot reduce costs efficiently and responds by cutting output — protecting the environment at the cost of economic activity.
2.  **R&D Reinvestment (Endogenous Growth Channel):** To avoid the output contraction trap, environmental tax revenues must be strategically reinvested in R&D, raising $A_V$. This drives down the convex cost curve of advanced recycling, transforming it from an elite option to the new operational standard. The two levers are therefore complementary, not interchangeable.

### Steady State Analysis
At steady state, system stability depends critically on the economy's emissions remaining below the environment's natural regeneration capacity. If emissions persistently exceed this threshold, pollution stock accumulates and erodes total factor productivity, eventually collapsing output. The model formally derives the conditions under which a stable, non-degenerative steady state exists — and shows these conditions require the policy mix above.

## Policy Implications

| Mechanism | Effect |
| :--- | :--- |
| **Environmental tax alone** | Reduces extraction, but risks output contraction without tech alternatives |
| **R&D investment alone** | Reduces recycling costs, but insufficient to correct extraction incentives |
| **Tax + R&D reinvestment** | Drives substitution toward advanced recycling, sustains output, reduces CRM dependency |
| **Technological progress in $A_V$** | Flattens recycling cost curve, making closed-loop economically dominant |

The model supports the CRMA's dual logic of regulatory targets + innovation funding, and suggests that carbon pricing instruments are most effective when revenue is hypothecated to circular economy R&D rather than general fiscal use. 

Beyond economics, the findings address an ethical contradiction in the green transition: clean downstream technologies (solar panels, EV batteries) built on environmentally and socially destructive upstream supply chains are not genuinely sustainable. Advanced recycling, by reducing virgin extraction dependency, offers a path toward coherence between climate objectives and supply chain responsibility.

---
**Repository Structure**
*   `README.md` — This file (model overview and results)
*   `Thesis_Francesca_Baglioni.pdf` — Full thesis
*   `Model_Derivations.pdf` — Formal mathematical derivations (FOCs, steady state)

**Author**
*Francesca Baglioni*
MSc Economics and Policy for Global Sustainability, Sapienza University of Rome
francesca.baglioni8@gmail.com
