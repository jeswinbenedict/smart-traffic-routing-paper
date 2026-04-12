<div align="center">

<h1>Intelligent Routing Protocols for Smart Traffic and Urban Mobility Networks</h1>

<p><strong>A first-principles technical analysis of what actually works in vehicular routing at city scale.</strong></p>

<p><em>"Conventional vehicular routing is broken. Build for the architecture that exists in 5 years, not the one that existed 5 years ago."</em></p>

<br/>

<img src="images/banner.png" width="100%" alt="Smart City Routing Network">

<br/><br/>

</div>

Modern cities regularly push arterial roads beyond 400–500 vehicles per kilometre. Traditional traffic management, designed for sparse and mostly unconnected fleets, collapses under this load. The result is familiar: gridlock, delayed safety messages, and fuel wasted at scale.

This work takes a first-principles view of routing in vehicular networks (VANETs): what fails, what scales, and what is realistically deployable in dense urban environments. The focus is on behaviour under real constraints—mobility, latency, density, and infrastructure—not on idealised simulations.

<div align="center">
<br/>
<img src="images/vehicle.png" width="80%" alt="Autonomous Vehicle Communication">
<br/><br/>
</div>

## Protocol Families at a Glance

Routing choices are grouped into four families, each with a clear operating envelope:

| Protocol Family                    | Strengths                    | Weaknesses                                | Verdict              |
|------------------------------------|------------------------------|-------------------------------------------|----------------------|
| Topology-Based (AODV, DSDV)       | Simple, well-studied        | Control overhead, collapses > 50 veh/km   | Legacy / fallback    |
| Geographic (GPSR, GyTAR)          | Low latency, scalable       | Needs maps, struggles in sparse networks  | Current best option  |
| Broadcast / Geocast               | Rapid safety dissemination  | Broadcast storms if unmanaged             | Safety-specific      |
| Learning-Based (Deep RL, etc.)    | Adapts to live conditions   | Training, sim-to-real gap, compute cost   | Emerging / near-term |

<div align="center">
<br/>
<img src="images/protocols.png" width="80%" alt="Routing Protocol Intelligence">
<br/><br/>
</div>

## What This Paper Shows

- **Geographic, road-aware routing** is the practical default for dense urban VANETs.  
- **Topology-based protocols** belong at the edges: stable backhaul, RSU meshes, and controlled corridors.  
- **Broadcast and geocast** must be engineered with storm-suppression; naïve flooding is untenable.  
- **Learning-based approaches** are promising, but bounded today by sim-to-real gaps and embedded inference limits.

## Measured Impact (from deployments and studies)

- Travel time reductions on coordinated “green wave” corridors in the range of **20–35%**.  
- Safety-critical alerts delivered in **sub‑100 ms** windows when routing is designed for latency first.  
- City-scale freight and fleet optimisation with **double‑digit percentage gains** in utilisation and fuel efficiency.

## Technology Stack Referenced

- Communication: **DSRC (IEEE 802.11p), C‑V2X, 5G NR‑V2X**  
- Network & simulation: **VANET, SUMO, OMNeT++ / Veins**  
- Protocols: **GPSR, AODV, GyTAR, VADD, geocast variants**  
- Intelligence: **Deep reinforcement learning, federated learning for routing policy adaptation**

---

<div align="center">

**A. Jeswin Karunya Benedict**  
Department of Computer Science and Engineering  
Vellore Institute of Technology, Andhra Pradesh, India  

<a href="https://github.com/jeswinbenedict">GitHub</a>

</div>
