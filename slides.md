---
layout: cover
class: text-center
title: Staking market
theme: academic
titleTemplate: '%s'
favicon: ./images/defiicon.png
author: Fayçal Drissi
themeConfig:
  paginationX: disabled
  paginationY: disabled
  paginationPagesDisabled: [1]
fonts:
  local: Montserrat, Roboto Mono, Roboto Slab # local fonts are used for legal reasons for deployment to https://slidev-theme-academic.alexeble.de and only set up for the example project, remove this line for your project to automatically have fonts imported from Google

mdc: true
---

## Blockchain Monetary Policy

Fayçal Drissi, Zachary Feinstein, Basil Williams

*University of Oxford, Stevens Institute of Technology, Imperial Business School*
<br>

<!--These slides: [https://www.faycaldrissi.com/siam2025](https://www.faycaldrissi.com/siam2025)
[my scholar](https://scholar.google.com/citations?user=njvyriQAAAAJ&hl=fr), 
[my website](https://www.faycaldrissi.com/), [my github](https://github.com/FDR0903)-->


---

# Overview

- Staking market
- Centralized / Decentralized Staking
- Is staking worth anything ?

---

<br /><br /><br /><br /><br /><br />
<p style="text-align: center;"><h1>
Issuance, staking, and DeFi <a name="defi"></a></h1>
</p>

---

# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 

---

# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 
* **Staking**: locking Eth in the blockchain to participate in the protocol: secure block production and validation

---


# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 
* **Staking**: locking Eth in the blockchain to participate in the protocol: secure block production and validation
* **Issuance**: rewards distributed by the protocol to incentivize staking

---


# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 
* **Staking**: locking Eth in the blockchain to participate in the protocol: secure block production and validation
* **Issuance**: rewards distributed by the protocol to incentivize staking
* These rewards are minted as new tokens and given to network participants who conduct consensus duties

---

# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 
* **Staking**: locking Eth in the blockchain to participate in the protocol: secure block production and validation
* **Issuance**: rewards distributed by the protocol to incentivize staking
* These rewards are minted as new tokens and given to network participants who conduct consensus duties
* **Burn**: gas fees are burned to use the blockchain

---

# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 
* **Staking**: locking Eth in the blockchain to participate in the protocol: secure block production and validation
* **Issuance**: rewards distributed by the protocol to incentivize staking
* These rewards are minted as new tokens and given to network participants who conduct consensus duties
* **Burn**: gas fees are burned to use the blockchain
$$\text{total supply of ETH} = \text{issuance} - \text{the burn (EIP-1559)}$$

---

# Issuance, staking, and DeFi
* **Blockchains** are distributed digital ledgers that **securely** store and execute transactions 
* **Staking**: locking Eth in the blockchain to participate in the protocol: secure block production and validation
* **Issuance**: rewards distributed by the protocol to incentivize staking
* These rewards are minted as new tokens and given to network participants who conduct consensus duties
* **Burn**: gas fees are burned to use the blockchain
$$\text{total supply of ETH} = \text{issuance} - \text{the burn (EIP-1559)}$$
* Last 30 days  
$$78,277.28 \text{ ETH issued} \qquad  8,041.75 \text{ ETH burned}$$

*Source: ultrasound.money*

---

# Issuance, staking, and DeFi
### Timeline of issuance

* **Jul 2015** Genesis: block reward set to 5 ETH (PoW miners were rewarded for producing blocks)
* **Oct 2017** Byzantium (EIP-649): block reward reduced to 3 ETH
* **Feb 2019** Constantinople (EIP-1234): block reward reduced to 2 ETH
* **Sep 2022** The Merge: Ethereum issuance is now only from PoS rewards (not withdrawable)
* **Apr 2023** Shanghai/Capella (EIP-4895): Withdrawals to the execution layer

---

# Issuance, staking, and DeFi
### Today

* Since the beacon chain: issuance is determined by an **issuance curve**
*  parameterized curve that calculates the *yield* as a function of the amount of ETH staked
$$
\text{yield} = \frac{2.6 \cdot 64}{\sqrt{\text{staked ETH}}}
$$

![issuancecurve](./images/issuancecurve.png){style="transform: translate(40%, 0%); width: 450px"}

---

# Issuance, staking, and DeFi
### Rationale
- Aim for 3.3% yield with 30 million ETH staked
- highly incentivizing at least 10 million staked ETH

![issuancecurve](./images/issuancecurve.png){style="transform: translate(60%, 0%); width: 400px"}

* **Issuance** in a blockchain is similar to **traditional monetary policy**

---

# Issuance, staking, and DeFi
### Today: staking high

- June 2025: 35 out 120 million ETH staked (88.6 bn $); stake rate of $28.24\%$
![stakinghistory](./images/stakinghistory.png){style="transform: translate(5%, 0%); width: 800px"}

---

# Issuance, staking, and DeFi
### Today: staking high

- June 2025: 35 out 120 million ETH staked (88.6 bn $); stake rate of $28.24\%$
![stakinghistory](./images/stakinghistory.png){style="transform: translate(5%, 0%); width: 800px"}



---

#  Research questions
- What are the equilibrium levels of staking and blockchain adoption ?
- Can equilibrium outcomes be controlled by the blockchain ? 
-  Can the Ethereum Foundation (EF) target objectives such as the volatility of the native token, economic security, and blockchain adoption ?
<br>


---

<br /><br /><br /><br /><br /><br />
<p style="text-align: center;"><h1>
Centralized / Decentralized staking
<a name="defi"></a></h1>
</p>


---

# The model

Two types of stakers: **whales** and **minnows**
- Initial ETH wealth of minnows: $s_{\text{g}}=s$
- Initial ETH wealth of whales: $s_{\text{w}}=m\,s$, $\qquad m \ge 1$

Relative risk aversion: $\gamma$

---

# The model

Two stage game

- **Stage one**: Whales and Guppies choose to enter the staking market
- **Stage two**: Whales and Guppies choose whether to stake in 
    - the Protocol Pool (PP)
    - the Liquid Pool (LP)
- The model is solve by backward induction

---

# Stage two

- $N^{\text{g}}$ minnows and $N^{\text{w}}$ whales are in the blockchain (determined endogenously in stage one)
- define $N$ as the number of equivalent minnows in the blockchain
$$
N = s\,N^{\text{w}} + N^{\text{g}}
$$
- $s_{\mathcal{P}}$ is the stake in the PP
- $s_{\mathcal{L}}$ is the stake in the LP
- The total stake is fixed
$$s_{\mathcal{L}}+s_{\mathcal{P}}=\overline{S}$$


---

# Stage two
### Protocol Pool

- Let $b$ a Bernoulli variable with parameter 
    $$\frac{s_{\mathcal{P}}}{s_{\mathcal{L}}+s_{\mathcal{P}}}$$
    - describes the probability that the protocol chooses a validator from the PP
- Let $f$ denote the fee for setting up a staking account
- The staking reward for type $i\in\{\text{g}, \text{w}\}$ in the PP
$$
R_{i}^{PP}=b\frac{s_i}{s_{\mathcal{P}}}R-f
$$

---

# Stage two
### Liquid Pool

- Let $\tilde{\sigma}$ be a normal rv with mean zero and std.dev $\sqrt{2\,\sigma}$
    - describes the uncertainty around LIDO's return (smart-contract risk)
- Let $\alpha$ be the performance fee taken by the LP
- The staking reward for type $i\in\{\text{g}, \text{w}\}$ in the LP
$$
R_{i}^{LP}=(1-b)\frac{s_i}{s_{\mathcal{L}}}\left(1-\alpha\right)R-\tilde{\sigma}
$$


---

# Stage two
### Protocol Pool

- For any concave utility $u$, and for type $i\in\{\text{g}, \text{w}\}$ in the PP we have 
$$
\begin{split}
\mathbb{E}\left[u\left(s_{i}+R_{i}^{PP}\right)\right]=&\frac{s_{\mathcal{L}}}{s_{\mathcal{L}}+s_{\mathcal{P}}}u\left(s_{i}-f\right)+\frac{s_{\mathcal{P}}}{s_{\mathcal{L}}+s_{\mathcal{P}}}u\left(s_{i}+\frac{s}{s_{\mathcal{P}}}R-f\right)\\=&\left(1-\frac{s_{\mathcal{P}}}{\overline{S}}\right)u\left(s_{i}-f\right)+\frac{s_{\mathcal{P}}}{\overline{S}}u\left(s_{i}+\frac{s}{s_{\mathcal{P}}}R-f\right)
\end{split}
$$

- So 
$$
\begin{split}
\partial_{s_{\mathcal{P}}}\mathbb{E}\left[u\left(s+R_{i}^{PP}\right)\right]=&-\frac{1}{\overline{S}}u\left(s_{i}-f\right)+\frac{1}{\overline{S}}u\left(s_{i}+\frac{s}{s_{\mathcal{P}}}R-f\right)-\frac{s\,R}{s_{\mathcal{P}}}\frac{1}{\overline{S}}\,u'\left(s_{i}+\frac{s}{s_{\mathcal{P}}}R-f\right)\\\le&0
\end{split}
$$
by concavity $u'\left(x+a\right)\le\frac{u\left(x+a\right)-u\left(x\right)}{a}$


---

# Stage two
### Equilibrium 

$$
\partial_{s_{\mathcal{P}}}\mathbb{E}\left[u\left(s+R_{i}^{PP}\right)\right]\le0
$$

- Strategic complementarity
- Any pure equilibrium is type-monotone
    - There is no interior pure Nash: at any interior split one side has a profitable deviation
- The same holds for LP

---

# Stage two
### Pratt’s approximation - risk premium

- Assume CRRA utility with aversion $\gamma$
- The (maximum) blockchain reward does not scale with the wealth
$$
\mathbb{E}\left[\frac{\left(s_{i}+\tilde{R}\right)^{1-\gamma}}{1-\gamma}\right]=\frac{s_{i}^{1-\gamma}}{1-\gamma}\mathbb{E}\left[\left(1+\tilde{R}/s_{i}\right)^{1-\gamma}\right]
$$

- The risk premium depends on the size of the reward relative to the initial wealth
- We use Pratt’s approximation of the risk premium for both types
$$
\begin{cases}
J^{PP,i}\left(s_{\mathcal{L}},s_{\mathcal{P}}\right) & =\mathbb{E}\left[u\left(s_{i}+R^{PP,\text{w}}\right)\right]\approx\mathbb{E}\left[R^{PP,i}\right]-\gamma^{i}\mathbb{V}\left[R_{i}^{PP,i}\right]\\
J^{LP,i}\left(s_{\mathcal{L}},s_{\mathcal{P}}\right) & =\mathbb{E}\left[u\left(s_{i}+R^{LP,\text{g}}\right)\right]\approx\mathbb{E}\left[R^{LP,i}\right]-\gamma^{i}\mathbb{V}\left[R^{LP,i}\right]-\gamma^{i}\,\sigma
\end{cases}
$$
where 
$$
\gamma^i = \gamma / s_i
$$

---

# Stage two
### Pratt’s approximation - risk premium

- For a type $i$, the objectives in both pools are
$$
\begin{cases}
J^{PP,i}\left(s_{\mathcal{L}},s_{\mathcal{P}}\right) & =\frac{s_{i}}{\overline{S}}R-f-\gamma^{i}R^{2}\frac{s_{i}^{2}}{\overline{S}^{2}}\frac{s_{\mathcal{L}}}{s_{\mathcal{P}}}\\
J^{LP,i}\left(s_{\mathcal{L}},s_{\mathcal{P}}\right) & =\frac{s_{i}}{\overline{S}}\left(1-\alpha\right)R-\gamma^{i}\left(1-\alpha\right)^{2}R^{2}\frac{s_{i}^{2}}{\overline{S}^{2}}\frac{s_{\mathcal{P}}}{s_{\mathcal{L}}}-\gamma^{i}\,\sigma
\end{cases}
$$

- We examine the following possible equilibria
    - all stakers go to LP
    - all stakers go to PP
    - whales go to PP, minnows go to LP
    - whales go to LP, minnows go to PP

---

# Stage two
### Simple case: $m=1$


---

# Stage two 
### All stakers go to LP ($\alpha=0$)
- In this case 
$$s_{\mathcal{L}}=\overline{S} \quad \text{and} \quad s_{\mathcal{P}}=0$$
- Deviation of a **minnow** leads to  $\quad s_{\mathcal{L}}=\overline{S}-s \quad \text{and} \quad s_{\mathcal{P}}=s$
- No deviation if 
$\qquad\qquad\qquad\quad
J^{PP,\text{g}}\left(\overline{S}-s,s\right)< J^{LP,\text{g}}\left(\overline{S},0\right)
$
- Deviation of a **whale** leads to  $\ \ \ \ s_{\mathcal{L}}=\overline{S}-m\,s \quad \text{and} \quad s_{\mathcal{P}}=m\,s$
- No deviation if 
$\qquad\qquad\quad\qquad
J^{PP,\text{w}}\left(\overline{S}-m\,s,m\,s\right)< J^{LP,\text{w}}\left(\overline{S},0\right)
$
- Equilibrium if
$$
\begin{cases}
-f+\gamma^{\text{g}}\,\left(\sigma-R^{2}\frac{N-1}{N^{2}}\right) & < 0\\
-f+\gamma^{\text{w}}\left(\sigma-R^{2}m\,\frac{N-m}{N^{2}}\right) & < 0
\end{cases}\quad  \underrightarrow{N\rightarrow\infty} \quad f>\gamma^{\text{g}}\sigma
$$

---

# Stage two 
### All stakers go to PP ($\alpha=0$)

- In this case 
$$s_{\mathcal{P}}=\overline{S} \quad \text{and} \quad s_{\mathcal{L}}=0$$
- Deviation of a **minnow** leads to  $\quad s_{\mathcal{P}}=\overline{S}-s \quad \text{and} \quad s_{\mathcal{L}}=s$
- No deviation if 
$\qquad\qquad\qquad\quad
J^{PP,\text{g}}\left(s,\overline{S}-s\right)< J^{LP,\text{g}}\left(0,\overline{S}\right)
$
- Deviation of a **whale** leads to  $\ \ \ \ s_{\mathcal{P}}=\overline{S}-m\,s \quad \text{and} \quad s_{\mathcal{L}}=m\,s$
- No deviation if 
$\qquad\qquad\quad\qquad
J^{PP,\text{w}}\left(m\,s,\overline{S}-m\,s\right)< J^{LP,\text{w}}\left(0,\overline{S}\right)
$
- Equilibrium if
$$
\begin{cases}
f & \le\gamma^{\mathrm{g}}\!\left(\sigma+\frac{R^{2}}{N^{2}}(N-1)\right)\\
f & \le\gamma^{\mathrm{w}}\!\left(\sigma+\frac{R^{2}}{N^{2}}\,m(N-m)\right)
\end{cases}\quad  \underrightarrow{N\rightarrow\infty} \quad f\le\gamma^{\mathrm{w}}\!\sigma
$$


---

# Stage two 
### Whales in LP, minnows in PP  ($\alpha=0$)

- No minnow wants to move PP$\to$LP and no whale wants to move LP$\to$PP iff

$$
\begin{cases}
f\; & \ge\;\gamma^{\mathrm{g}}\!\left(\frac{R^{2}}{N^{2}}-\frac{R^{2}}{N^{2}}\frac{N^{\mathrm{g}}-1}{N^{\mathrm{g}}+1}-\sigma\right)\\
f\; & \le\;\gamma^{\mathrm{w}}\!\left(\sigma+\frac{m^{2}R^{2}}{N^{2}}\frac{2}{N^{\mathrm{w}}+1}\right)
\end{cases}
$$

---

# Stage two 
### Whales in PP, minnows in LP  ($\alpha=0$)

- No minnow wants to move PP$\to$LP and no whale wants to move LP$\to$PP iff

$$
\begin{cases}
f\; & \ge\;\gamma^{\mathrm{w}}\!\left(\frac{R^{2}}{N^{2}}-\frac{R^{2}}{N^{2}}\frac{N^{\mathrm{g}}-1}{N^{\mathrm{g}}+1}-\sigma\right)\\
f\; & \le\;\gamma^{\mathrm{g}}\!\left(\sigma+\frac{m^{2}R^{2}}{N^{2}}\frac{2}{N^{\mathrm{w}}+1}\right)
\end{cases}
$$

---

# Stage one 
- Stakers decide whether to invest in a risk-free asset $r^\$$ or enter the blockchain
- 


---

<br /><br /><br /><br /><br /><br />
<p style="text-align: center;"><h1>
Is staking worth anything ? <a name="defi"></a></h1>
</p>


---

# short answer
NO


---

# TO say 
what would stop it:
- diversification of pools: more liquidity costs -> prefer using ETH
- small rewards -> such that it's smaller than 

---

# TO SAY:

### DVT: distributed validator technology
### Solo staking: an impossibility, any pool is strictly preferable
https://vitalik.eth.limo/general/2023/09/30/enshrinement.html
https://notes.ethereum.org/bW2PeHdwRWmeYjCgCJJdVA

---

---
layout: end
---

Thank you !

[faycaldrissi.com](https://www.faycaldrissi.com/)
