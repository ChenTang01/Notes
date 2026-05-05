# Notes

- **Reducing Traffic Incidents in Meal Deliveries: Penalize the Platform or Its Independent Drivers?** MSOM (2026) Wenchang Zhang, Christopher S. Tang, Liu Ming, Yue Cheng

  - The main conclusion is that ==*penalizing the platform is more effective than directly penalizing drivers in reducing meal-delivery traffic incidents.*==
  - The key mechanism is that unsafe driving is not modeled as purely driver-initiated behavior. Instead, it is induced by the platform’s aggressive delivery-time promises and commission design.
  - The model has four parties: the government, the platform, customers, and independent drivers.
    - The government first chooses the penalty scheme $(A,R)$, where $A$ is the penalty on drivers and $R$ is the penalty on the platform.
    - The platform then observes $(A,R)$ and customer type $(x,v)$, and chooses the delivery fee $kx$ and driver commission $bx$ to maximize expected profit.
    - The customer utility is $\sigma(x,v,k,t)=v-kx-\beta t$, where $x$ is delivery distance, $v$ is meal valuation, $kx$ is the delivery fee, and $\beta t$ is waiting-time disutility.
    - The driver chooses whether to accept the order and how fast to deliver. The driver’s expected earning rate is $u(t;b,x,A)=(1-G(t;x))bx/t-G(t;x)A$, where $G(t;x)$ is the incident probability.
    - The platform profit is $\pi=(1-G(t;x))[\gamma+(k-b)x]-G(t;x)R$, where $\gamma$ is the platform’s restaurant-side revenue and $R$ is the platform penalty after an incident.
    - The government maximizes total social surplus, which includes platform profit, customer surplus, driver earnings, and public safety benefits: $S=\pi^*+\sigma^*+u^*T^*+(1-G(T^*))P$.

  

- **Evolution of Ride Services: From Ride Hailing to Autonomous Vehicles** MS (2026) Daehoon Noh, Tunay I. Tunca, Yi Xu 

  - Perfect characterization between the AV model and RH model:

    - **AV model**: Its main decisions are capacity $K$ and price $p_V$. Supply is fixed by its own investment, so $S_V=K$, and profit is $\Pi_V=(p_V-c_V^o)D_V-c_fK$. The key feature is fixed capacity investment: AV has direct control over supply but must bear the upfront capacity cost $c_fK$.

    - **RH model**: The RH firm is a ride-hailing platform that does not own vehicles. Its main decisions are the driver revenue share $\alpha$ and price $p_R$. Supply $S_R$ is induced through drivers’ participation decisions, where driver payoff is $(\alpha p_R-c_R^o)D_R/S_R$, and platform profit is $\Pi_R=(1-\alpha)p_RD_R$. The key feature is flexible supply adjustment through $\alpha$.
  
  
    - **Consumer choice**:  utility is $u_C=a-p_i-bD_i/S_i$, where $p_i$ is price and $D_i/S_i = W(D,S)$ captures waiting cost.
  
    - ==Deserved Extending==: A mixed AV and human driver business model in which a platform can host AVs owned by a third party.
