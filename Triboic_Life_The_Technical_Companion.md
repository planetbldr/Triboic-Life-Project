# Triboic Life: The Technical Companion

## Europa Fulgorax — Human-Readable Technical Companion (REP-B1)

**Daniel Moskal**  
**Project:** Europa Triboheterotroph / Triboic Life  
**Publication version:** 1.0  
**Publication freeze:** 2026-09-26  
**Publication set:** [*Life Powered Like Lightning*](Life_Powered_Like_Lightning_FINAL_2026-09-26.md) · [*The Triboic Frontier*](The_Triboic_Frontier_FINAL_2026-09-26.md) · [*Triboic Life: The Technical Companion*](Triboic_Life_The_Technical_Companion_FINAL_2026-09-26.md)  
**Canonical science base lock:** 2026-09-12  
**FMC science amendment:** 2026-09-24  
**HR5 human-style revision:** 2026-09-26  
**Report status:** OWNER-APPROVED HUMAN-READABLE TECHNICAL COMPANION  
**Scientific state:** DESK-SCIENCE COMPLETE WITH EXPLICIT EMPIRICAL UNRESOLVEDS

---

## Contents

### Part I — The Idea and the Machine
- TC-00 — How to Read This Companion
- TC-01 — What the Project Actually Concluded
- TC-02 — The Europa Environment: A Conditional Test Scenario
- TC-03 — K1: The Tribowhip Architecture
- TC-04 — From Moving Water to Useful Electricity: The Missing Bridge
- TC-05 — Electrochemistry: Making Oxygen Without Free Oxygen

### Part II — Building a Whole Organism
- TC-06 — Oxygen Demand, Respiration, and Gas Handling
- TC-07 — Eating in the Dark: Prey, Farming, and Sustainable Supply
- TC-08 — Durability, Repair, Development, Reproduction, and Organization

### Part III — How Large, and What Kind of Fulgorax?
- TC-09 — The Smallest Fulgoray We Could Defend
- TC-10 — How Large Could a Fulgorax Become?
- TC-11 — The Four Europa Fulgorax Forms
- TC-12 — What Nature Already Does — and What It Does Not

### Part IV — Detection, Earth Experiments, and the Research Roadmap
- TC-13 — Chemistry, Biosignatures, and the Direct Test
- TC-14 — The Earth Diffuse-Vent Experimental Program
- TC-15 — What We Need to Know Next

### Part V — Methods, History, and What Survives
- TC-16 — Methods, Computation, and Reproducibility
- TC-17 — How the Creature Changed
- TC-18 — What Survives the Analysis
- TC-19 — How Many Bodies Have Moving Fluids?

### Appendices
- APP-A — CCID Master Index
- APP-B — Primary Source and Citation Register
- APP-C — `[SIM]` / Run Provenance Register
- APP-D — Equation / Model / Parameter Register
- APP-E — Fulgora Nomenclature and Technical Crosswalk
- APP-F — Historical / Superseded / Nonportable / VOID Register
- APP-G — Empirical Frontier / STOP / Future-Model Register
- APP-H — Reproduction and Audit Checklist
- Canonical Lock Record — REP-B1 / FMC-14 Science Amendment

---

## Canonical-status note

This document is the human-readable Technical Companion for the Europa Fulgorax project. The 2026-09-12 canonical base consolidates the owner-approved REP-B1 scientific state, and the 2026-09-24 FMC amendment adds the Fluid-Motion Census framework without altering the earlier Europa organism science. The 2026-09-26 HR5 revision is a prose and readability revision only. It does not silently upgrade, downgrade, or replace the underlying scientific dispositions.

This remains a synthesis and reference document. It adds organization, explanation, cross-reference, and auditability. The Europa scientific truth layer remains the frozen project state established by C-final, MS11, BC, FC7, NR, METH, and the final claim/citation/[SIM] freeze, with the later FMC-14 census layer controlled separately.

The integrated Fulgorax architectures remain **[SPEC-INTEGRATED]**. No integrated organism has been observed, built, cultured, or experimentally demonstrated.

The governing report rule is:

> **A more detailed explanation may reveal more uncertainty, provenance, and mechanism. It may not silently upgrade what the project established.**

---

# Part I — The Idea and the Machine

## TC-00 — How to Read This Companion

This report is the technical counterpart to *Life Powered Like Lightning*. The accessible report tells the story of the project; this companion exposes the machinery underneath it: the environmental assumptions, candidate organs, calculations, empirical analogues, branch logic, failed paths, unresolved measurements, and the reasons some apparently attractive simulations were deliberately not run.

The most important discipline in reading a project like this is to keep different kinds of evidence separate. A component can have strong experimental precedent without the complete organism being demonstrated. A simulation can be numerically precise while depending on uncertain biological inputs. A design choice can be reasonable without being uniquely required by the science. This companion therefore keeps five evidence categories visible throughout.

- **[LAB]** — a claim supported by external empirical work at the claim level. The primary paper or dataset is the authority, not this project's restatement of it.
- **[SIM]** — a quantitative result that was actually executed and retained under the project's computational controls. An equation, planned calculation, or unexecuted model is not `[SIM]`.
- **[SPEC]** — reasoned scientific speculation or extrapolation that has not been established empirically.
- **[SPEC-CHOICE]** — an explicit project design or modeling choice selected from more than one plausible alternative.
- **[SPEC-INTEGRATED]** — a complete architecture assembled from components that may individually have stronger support, but whose integration has not itself been demonstrated.

Evidence class and applicability are separate questions. A laboratory result may be excellent `[LAB]` evidence for the phenomenon it measured while remaining only an analogue for Europa. The project therefore also distinguishes direct applicability, analogue applicability, partial applicability, known mismatch, and unresolved applicability.

This separation prevents one of the easiest mistakes in speculative engineering: **evidence aggregation**. If every part of an organism has some precedent, it is tempting to treat the assembled organism as though it also has precedent. That inference is not allowed here. The final Europa organisms remain `[SPEC-INTEGRATED]` even when individual mechanical, electrochemical, metabolic, or ecological components are supported by stronger evidence.

### Project-state terminology

The project also distinguishes scientific status from evidence type. The terms **current**, **historical**, **superseded**, **nonportable**, **failed/noncanonical**, and **VOID** have specific meanings.

- **Current** means authoritative within its stated scope.
- **Historical** means accurate as a record of what the project once tested, assumed, or concluded.
- **Superseded** means later controlled work replaced it as current authority.
- **Nonportable** means a result can remain valid in the topology or model that produced it while being unusable elsewhere.
- **Failed/noncanonical execution** means computation occurred but did not earn scientific-result authority.
- **VOID** means a numerical result is quarantined and may not be reused.

These distinctions matter because an older result is not automatically false, and a numerically valid result is not automatically portable. Much of the Europa execution involved discovering exactly where a result remained valid and where later architectural changes made reuse inappropriate.

### Permanent interpretation firewalls

Several distinctions recur so often that they should be treated as permanent reading rules:

\[
Q_{\mathrm{separated}} \neq Q_{\mathrm{usable}}
\]

\[
I_{\mathrm{separated}} \neq I_{\mathrm{usable}}
\]

\[
\text{PREY DENSITY} \neq \text{PREY SUPPLY RATE}
\]

\[
\text{C1 lifetime scenario} \neq \text{empirical K1 lifetime}
\]

\[
\text{energy autonomy} \neq \text{matter autonomy}
\]

\[
\text{valid in one topology} \neq \text{numerically portable to another topology}
\]

The later Fluid-Motion Census adds another firewall:

\[
N_{\rm FM}
\neq
N_{\rm habitable}
\neq
N_{\rm inhabited}
\neq
N_{\rm intelligent}
\neq
N_{\rm detectable\ civilizations}
\]

The first group protects the organism model from common category errors. Charge separation is not the same as useful current delivered through a load. A measured prey concentration is not the same as a sustainable replenishment rate. A modeled lifetime scenario does not become an empirical durability measurement. A branch that becomes energetically independent can still depend on external carbon, nutrients, or other matter. A result derived for one architecture cannot be carried into another merely because both are called Fulgorax.

The final firewall performs the same function at planetary scale. The Fluid-Motion Census counts physical opportunity for substantial persistent or recurrent moving fluids. It does not count habitable worlds, inhabited worlds, intelligent life, or detectable civilizations.

This report repeatedly states what a result **does not establish** because those nonclaims are part of the scientific result. A boundary on interpretation is not editorial caution added after the work; it is part of what the work concluded.

### Naming used in this report

The broad hypothetical class is **triboic life**. The defining energy-acquisition strategy is **tribotrophy**, and a generic organism using that strategy is a **tribotroph**. **Fulgorax** is the project/common name for a hypothetical triboic organism rather than a formal biological taxon. The name derives from *Fulgora*, a Roman personification of lightning, with the final *x* treated as a wildcard.

The four final Europa architectures are:

- **Fulgoray** — M0-HET, the reference heterotrophic consumer.
- **Fulgorad** — M3-Dmix, the electrically subsidized consumer.
- **Fulgoral** — M3-DA-U, the direct host producer.
- **Fulgoraz** — M3-IS(O), the internal electro-symbiotic producer.

These names identify alternatives, not a ladder. They do not imply increasing sophistication, evolutionary sequence, or increasing maximum size.

### Technical Trace — TC-00

**Project authority:** AP-CTRL, AP-FZ, AP-METH, AP-FMC14  
**Evidence rule:** primary sources for external empirical claims; project artifacts for project-state claims  
**Whole-creature status:** `[SPEC-INTEGRATED]`  
**Permanent firewalls:** useful charge, lifetime, prey supply, topology portability, no invented minimum or maximum

---

## TC-01 — What the Project Actually Concluded

The project did not prove that triboic life exists, that Europa contains life, or that the proposed organism can be built. It did not construct a tribowhip, measure useful K1 current, establish an empirical K1 lifetime, or derive a numerical minimum or maximum body size.

What it did was narrower and more useful: it took one speculative energy-acquisition mechanism—environmental motion driving repeated contact electrification in biological structures—and tested whether a specific Europa organism concept could remain internally coherent once mechanical, electrical, metabolic, ecological, scaling, repair, and developmental constraints were considered together.

The final result can be summarized in four layers. The first three concern the Europa organism itself. The fourth concerns the broader physical opportunity for moving-fluid environments beyond Europa.

### First: a conditional minimum reference survived desk-science integration

For the original heterotrophic branch, Fulgoray, the final whole-creature integration retained one minimum-complexity reference family that was not eliminated by the executed constraints:

> **C8-U / H5-U CONDITIONAL REFERENCE FAMILY**

Its formal disposition is:

> **UNRESOLVED-EMPIRICAL / DESK-SCIENCE COMPLETE**

This does not mean a working minimum organism was demonstrated. It means that, within the scope actually executed, the integrated analysis did not expose a contradiction that eliminated every admissible realization of the reference family.

No exact scalar minimum was earned. The minimum result is therefore a **family of biological and architectural requirements**, not a millimeter value. Earlier specific dimensions should not be interpreted as current minimum anatomy.

### Second: maximum-size analysis did not earn a maximum

The MS11 maximum-size phase reached an equally constrained conclusion. It did **not** establish:

1. a numerical maximum size;
2. unlimited growth;
3. one unique first-failing constraint; or
4. evidence that Fulgorad, Fulgoral, or Fulgoraz has a larger maximum size than Fulgoray.

Maximum size is therefore represented as a **joint-admissibility boundary**. The organism reaches that boundary only when no authorized morphology, modular organization, or biological realization can satisfy all mandatory constraints at the same time.

Across the retained architectures, the strongest shared structural backbone is:

\[
\{K,A,R\}
\]

where:

- **K** = K1 deployment, support, source, and useful-transfer burden;
- **A** = anchoring force and moment burden;
- **R** = durability, repair, and replacement burden.

This set is structurally implicated across the scaling analysis. It was not established as a statistically demonstrated unique first failure.

### Third: the project ended at an empirical frontier

The most important unresolved architecture-level question is EF-1:

> **Can the actual hydrated sealed K1 architecture repeatedly export useful charge under load, close its return/reset problem, and recover for another cycle?**

That question now matters more than extending the organism model with additional speculative precision. If EF-1 succeeds, measured source behavior can replace assumed source families and make downstream work more meaningful. If repeated testing shows that the authorized sealed-K1 mechanism family cannot produce useful loaded charge and reset reproducibly, the correct response is:

> **STOP / OWNER-CONTROLLED REDESIGN**

A failed source mechanism cannot be rescued by adding more tribowhips, enlarging the creature, or making the metabolism more elaborate. The generator would have to change.

### Fourth: the physical opportunity space is broader than Europa, but no census scalar was earned

The later Fluid-Motion Census asked a different question from the organism-design work:

**How many physically distinct bodies may possess at least one substantial moving-fluid environment?**

That quantity is denoted \(N_{\rm FM}\). It represents physical opportunity for macroscopic fluid motion, not the number of habitable worlds and not the number of environments in which triboic life is expected to occur.

FMC-14 did not support one preferred Milky Way value for \(N_{\rm FM}\). Some populations have comparatively strong physical evidence for moving fluids but weak Galactic normalization. Other populations are abundant but have uncertain fluid-bearing fractions. Moons, dwarf or minor planetary bodies, and several compact-host populations remain demographically incomplete. The appropriate result is therefore a modular census framework in which unresolved terms remain symbolic rather than being forced into one apparently precise number.

The FMC work broadens the **physical context** of Triboic Life without strengthening the biological claim. Fulgorax remains `[SPEC-INTEGRATED]`, and EF-1 remains the first architecture-level empirical test.

### Technical Trace — TC-01

**Primary CCIDs:** CC-CFINAL-01, CC-MS11-01, CC-EF1-01, CC-FUTSIM-01, CC-FMC-01, CC-FMC-BIO-01  
**Project authority:** AP-CFINAL, AP-MS11, AP-NR, AP-FZ, AP-FMC14  
**Prohibited stronger reading:** “the creature works,” “the project proved triboic life is viable on Europa,” or “the FMC count is a count of habitable or inhabited worlds”

---

## TC-02 — The Europa Environment: A Conditional Test Scenario

The project does not claim that an inhabited hydrothermal vent has been observed on Europa. Europa is used as a demanding **conditional environment** in which to test the architecture: a cold, saline, high-pressure ocean beneath an ice shell, with possible seafloor water-rock interaction and potentially localized hydrothermal circulation.

The organism is therefore evaluated **conditional on** a mechanically usable local flow niche and a chemically appropriate environment existing. This is an important distinction. The report tests whether the organism can survive a specified environmental scenario; it does not convert that scenario into a claim that the corresponding Europan habitat has been observed.

The environmental model separates three evidentiary layers:

1. **Target-system evidence** — spacecraft observations, geophysical models, geochemical constraints, and planetary-science work relevant to Europa.
2. **Earth analogues** — especially diffuse hydrothermal systems that provide empirical information about low-velocity aqueous flow, redox gradients, microorganisms, material transport, and related processes.
3. **Project scenario choices** — specific local environmental conditions selected so that the organism can be tested quantitatively.

That separation prevents Earth analogue values from silently becoming measurements of Europa.

### Temperature and local environment

The project's nominal ice-ocean boundary reference of approximately **268–273 K** is not a claim that the hypothetical seafloor habitat sits at that temperature. Local vent, reactive-subsurface, or water-rock-interaction environments may differ substantially from the bulk ocean and from conditions near the ice-ocean interface.

The working organism scenario therefore depends on a set of explicit environmental assumptions rather than one globally assigned Europan state:

- locally anoxic or oxygen-poor conditions;
- liquid water or brine;
- high pressure;
- persistent or recurrent local fluid motion capable of driving compliant structures;
- a mineral or other substrate that allows attachment for the sessile reference organism;
- access to matter and, for Fulgoray, biological prey or prey-equivalent reduced material.

These are design inputs to the conditional test scenario. They are not observations of a known Europan biosphere.

### The flow assumption

Flow is especially important because the energy source begins with mechanical motion. Earth diffuse-vent observations establish that sustained low-velocity aqueous flow exists as a real mechanism class. They provide useful physical and ecological analogues for what moving water can do in a chemically active seafloor environment.

They do **not** establish Europa's local velocity field.

The project therefore uses Earth diffuse-flow measurements and related literature to constrain plausible mechanism classes and reference regimes, while keeping the Europan flow itself a conditional scenario input. Treating an Earth vent velocity as a direct Europan measurement would be a category error.

### What the environmental step did not establish

The Europa environment work did not establish that hydrothermal activity is occurring at a particular site today, that microbial prey exist there, or that the selected flow regime is common. It also did not show that final K1 materials tolerate every plausible Europan brine composition, nor that a Fulgorax could be detected remotely from Europa's surface.

The environmental step instead established a controlled conditional scenario within which the organism could be tested. That is enough for the purpose of the project, but it should not be read as an observed habitat.

### External source package

**SP-ENV-01** retains Europa ocean, interior, and geochemistry modeling, including [Vance et al. (2018)](https://doi.org/10.1002/2017JE005341), [Vance et al. (2021)](https://doi.org/10.1029/2020JE006418), [Spiers & Schmidt (2023)](https://doi.org/10.1029/2023JE008028), [Marion et al. (2005)](https://doi.org/10.1016/j.gca.2004.06.024), [Nozaki et al. (2025)](https://doi.org/10.1016/j.pepi.2025.107450), and [Byrne et al. (2026)](https://doi.org/10.1038/s41467-025-67151-3).

**SP-FLOW-01** retains Earth diffuse-flow analogue work, including [Mittelstaedt et al. (2012)](https://doi.org/10.1029/2011GC003991) and [Mittelstaedt et al. (2016)](https://doi.org/10.1002/2015GC006144).

These source-package mentions are kept traceable through ordinary Markdown bibliography entries or direct links rather than platform-specific citation objects.

### Technical Trace — TC-02

**Primary CCID:** CC-ENV-01  
**Evidence:** `[LAB]` / model literature for environmental constraints and Earth analogues; `[SPEC-CHOICE]` for the integrated local scenario  
**Applicability:** target-system modeled/partial plus Earth analogue  
**Prohibited stronger reading:** “Europa has the habitat used in this report.”

---

## TC-03 — K1: The Tribowhip Architecture

K1 is the project's central candidate power organ: a compliant, sealed biological appendage in which environmental motion drives repeated internal contact and separation. The active triboelectric interface is therefore not assumed to sit directly in conductive seawater. Mechanical forcing comes from the external fluid, while the charge-generating surfaces remain inside a contained biological structure.

That distinction changes the engineering problem. The relevant question is not whether an exposed dry triboelectric material can retain charge underwater. It is whether a hydrated biological structure can keep an internal contact-separation process isolated enough to generate charge, transfer that charge into useful electrochemistry, close the countercharge path, reset, and repeat while being mechanically driven from outside.

### K1 is function-first, not a frozen anatomy

The final K1 representation assigns required functions rather than a final layer stack. Its major functional regions are:

- biological outer seal or containment;
- compliant structural support or backing;
- hydrated cellulose-class triboelectric contact function;
- internal contact-separation region;
- quinone/redox/buffering function;
- electrical or conductive routing to downstream electrochemistry.

The exact order, sidedness, polarity, thickness, cavity geometry, conductor placement, and final material arrangement remain unresolved. A diagram showing these regions should therefore be read as a functional map rather than a cross-section of established anatomy.

Cellulose-class materials remain attractive because cellulose has empirical triboelectric precedent ([Zhang et al. 2020](https://doi.org/10.1002/adma.202002824)) and because biological systems can manufacture cellulose-like structural polymers. Quinones remain attractive because they are widespread redox-active biological molecules with strong electrochemical precedent; the retained project package includes quinone/polyquinone and redox-polymer analogues ([Illera-Perozo et al. 2022](https://doi.org/10.1039/D2RA01232D); [Bertaglia et al. 2024](https://doi.org/10.1002/admt.202400623); [Tang & Ng 2017](https://doi.org/10.1016/j.biortech.2017.07.189); [Milton et al. 2015](https://doi.org/10.1039/C5SC01538C)). Those facts support individual functions in the proposed architecture; they do not establish the integrated K1 mechanism.

No retained primary study demonstrates the complete sequence

\[
\text{hydrated cellulose-class contact}
\rightarrow
\text{useful charge transfer}
\rightarrow
\text{quinone/redox capture}
\rightarrow
\text{countercharge closure}
\rightarrow
\text{reset}
\]

in the actual K1 architecture. That missing demonstration is the central empirical gap, not an omission that can be repaired by adding more references.

### Mechanics and source opportunity

P0-B deliberately treated K1 as a **family of architectures** rather than one fixed geometry. The retained source-side work explored low-flow compliant mechanics, contact opportunity, cycle-rate sensitivity, real-contact-fraction sensitivity, separated charge, separated current, and conditional source power.

Those screens produced a **source-side conditional pass**. Within the modeled parameter space, there remained broad regions in which flexible underwater K1-like structures could deform and generate separated charge. That result keeps the mechanical-source concept open, but it does not establish useful electrical closure.

This distinction becomes important throughout the project. K1 can survive a mechanical and raw-charge screen while still failing as a power organ if the separated charge cannot be transferred through a biological load and the system cannot recover for another cycle.

### Finite physical thickness

The maximum-size work also imposed a basic physical constraint:

\[
h_{K1} \ge h_{K1,\min} > 0
\]

No numerical value for \(h_{K1,\min}\) is currently adopted.

The purpose of this inequality is not to assign a minimum tribowhip thickness. It prevents a scaling model from obtaining arbitrarily large functional area at zero structural cost by allowing K1 elements to become infinitely thin. Any real generator must occupy finite material volume and carry corresponding construction, support, durability, and hydrodynamic costs.

### Technical Trace — TC-03

**Primary CCID:** CC-K1-ARCH-01  
**Project authority:** AP-CFINAL, AP-MS11, AP-FZ  
**External packages:** SP-P0B-01, SP-EF1-01  
**Integrated K1 status:** `[SPEC-INTEGRATED]`  
**Final geometry:** unresolved  
**Final polarity:** unresolved  
**Final useful-transfer efficiency:** unresolved

---

## TC-04 — From Moving Water to Useful Electricity: The Missing Bridge

![TC-01 — K1: From Motion to Useful Power?](../figures/LP02_TC01_K1_MOTION_TO_USEFUL_POWER_FINAL_2026-09-26.png)

*Figure TC-01 / LP-02 — K1: From Motion to Useful Power? Conceptual K1 schematic; not canonical anatomy. Exact spatial arrangement, material order, dimensions, polarity, gap geometry, and routing remain unresolved. EF-1 — useful transfer under a real load plus repeatable reset — has not been experimentally demonstrated; the reset loop is a required cycle, not an achieved result.*

The central electrical problem can be stated simply:

> **Making charge is not the same thing as powering biology.**

A tribowhip can separate charge and still fail completely as a biological power organ. The project therefore keeps the physical sequence explicit:

\[
\text{flow}
\rightarrow
\text{deformation}
\rightarrow
\text{contact}
\rightarrow
\text{separation}
\rightarrow
Q_{\rm separated}
\rightarrow
I_{\rm separated}
\rightarrow
\text{useful loaded transfer}
\rightarrow
\text{electrochemistry}
\]

Mechanics, triboelectric analogue data, and source-side computation can investigate much of the chain through separated charge and current. The transition from separated charge to repeatable useful loaded transfer is the unresolved bridge addressed by EF-1.

### P0-B — source-side opportunity

The retained P0-B runs, including SIM-EU-02 through SIM-EU-05, explored source-side behavior rather than completed biological power delivery. They addressed low-flow deformation opportunity, candidate contact and cycle behavior, separated charge and current, and conditional source power at specified voltage.

These are legitimate `[SIM]` results within their scope. They do **not** demonstrate that the biological redox system can accept the generated charge, maintain the required potential, close countercharge, or recover after transfer.

### P0-C — required fraction, not achieved efficiency

P0-C was designed specifically to avoid inventing an interface efficiency.

Instead of assuming that some arbitrary percentage of separated charge becomes useful, the calculation asked how much of the modeled raw source would need to become useful for the candidate array to meet the biological oxygen demand:

\[
u_{\rm required}
=
\frac{I_{\rm required}}
{I_{\rm separated,array}}
\]

SIM-EU-06 mapped that required fraction across the retained biological-demand and source states. The result tells us the performance the interface **would need** to achieve for closure under each modeled condition. It does not tell us what the interface **does** achieve.

The permanent firewall is therefore:

\[
u_{\rm required}
\neq
\eta_{\rm interface,achieved}
\]

No numerical value for \(\eta_{\rm interface}\) is currently authorized.

This is one of the most important methodological controls in the project. Without it, a calculated requirement can quietly become an assumed biological efficiency and then propagate through downstream sizing as though it had been measured.

### Temporal conditioning — IC-5

A large K1 array does not have to operate with every tribowhip in perfect phase. SIM-EU-11 explored phase staggering and partial-to-full synchronization as a sensitivity problem.

The result supports a qualitative opportunity for temporal smoothing: asynchronous source elements could reduce the extreme pulsatility of the array-level raw source. It does not demonstrate a real biological capacitor, establish a final buffering mechanism, or show that useful current remains smooth after the unresolved EF-1 transfer losses are included.

### Anchoring — Gate E

SIM-EU-08 through SIM-EU-10 explored array loading, force per attachment area, and holdfast moment within the tested reference space. Those screens did not expose a minimum/reference anchoring kill.

That is not the same as demonstrating a finished holdfast. Final attachment chemistry, fatigue life, substrate interaction, repair, and morphology remain unresolved. The Gate E result says only that anchoring did not become a forced desk-science contradiction within the modeled opportunity space.

### EF-1 — the architecture-existential experiment

EF-1 must test a sufficiently representative hydrated, sealed K1 system through a complete repeated cycle:

1. mechanical forcing and contact/separation;
2. separated charge;
3. electrical export through a controlled load;
4. redox capture or routing;
5. countercharge closure;
6. reset;
7. reproducibility over many cycles.

A one-time voltage spike is insufficient because it establishes only that charge separation occurred. A generic triboelectric nanogenerator is insufficient because it does not reproduce the biological containment, redox, and reset problem. Likewise, demonstrating that a quinone can be electrochemically reduced or oxidized in isolation does not demonstrate that the K1 system can couple triboelectric generation into that chemistry repeatedly.

The integrated cycle is the missing bridge.

A lower-than-hoped but reproducibly nonzero useful-transfer relation would not automatically kill the architecture. Once measured, that value could replace the unknown interface performance and the downstream organism could be recalculated around it. Required K1 area might increase, some morphologies might become unattractive, or some higher-demand services might no longer close.

A mechanism-level failure is different. If the retained sealed-K1 family cannot export useful loaded charge and recover reproducibly, the current K1 architecture stops. Downstream biological complexity cannot repair a failed source mechanism.

### Technical Trace — TC-04

**Primary CCIDs:** CC-EF1-01, CC-P0B-01, CC-P0C-01, CC-E-01, CC-IC5-01  
**Current `[SIM]`:** SIM-EU-02 through SIM-EU-06, SIM-EU-08 through SIM-EU-11  
**Global unresolved:** EF-1  
**Prohibited interpretations:** \(Q_{\rm separated}=Q_{\rm usable}\), \(I_{\rm separated}=I_{\rm usable}\), or any invented numerical interface efficiency

---

## TC-05 — Electrochemistry: Making Oxygen Without Free Oxygen

Baseline Fulgoray uses oxygen as a respiratory oxidant while being modeled in a locally anoxic or oxygen-poor environment. The architecture does not solve that problem by assuming an unobserved oxygen reservoir. It proposes that the organism manufacture oxygen internally through electrically driven water oxidation.

The idealized oxygen-evolution half-reaction is:

\[
2H_2O \rightarrow O_2 + 4H^+ + 4e^-
\]

with complementary reduction chemistry providing the cathodic side of the circuit. For the baseline retained water-splitting topology, the ideal stoichiometric overall relation is:

\[
2H_2O \rightarrow O_2 + 2H_2
\]

The oxygen is biologically useful to Fulgoray because it supports respiration. Hydrogen appears as the complementary coproduct in the retained baseline topology; its ecological or metabolic reuse is a separate question rather than free credit to the organism.

### B1 — catalyst-family feasibility

The catalyst literature establishes multiple oxygen-evolution and hydrogen-evolution mechanism classes, including families with biological or biomimetic relevance. The project did not identify a catalyst-family contradiction at the desk-science level that independently forces the architecture to fail.

That is a limited result. Demonstrating relevant catalytic mechanisms does not demonstrate an integrated biological electrolyzer operating at low temperature, high pressure, inside a sealed living architecture with compatible catalysts, supports, separators, conductors, membranes, and repair systems. Those integrated implementation questions remain conditional.

### Repaired B2 operating requirement

The earlier Gate-A/B2 history included a scalar comparison between food energy and electrolysis cost. That framing was later superseded because it combined resource ledgers that should remain separate.

The repaired B2 result instead asks directly what electrochemical operating requirement the selected reaction system imposes. SIM-EU-14 gives the retained pH-7 core modeled requirement:

\[
V_{\rm core,pH7}
=
1.824809932\ {\rm V}
\]

before routing sensitivity.

The full numerical precision is retained because it is the exact output of the model. It should not be interpreted as matching biological precision. This is not a measured K1 voltage, not an experimentally demonstrated operating point, and not evidence that a Fulgorax can actually sustain that potential.

### Keep the resource ledgers separate

The mature architecture distinguishes at least three accounting streams:

1. **flow-derived electrical service**;
2. **food-derived metabolic carbon and chemical energy**;
3. **material construction, maintenance, and repair**.

For baseline Fulgoray, prey supplies reduced carbon, nutrients, and biological matter. K1-derived electricity chiefly supplies the electrical service needed for oxidant production and related electrochemistry.

Keeping these ledgers separate prevents a conceptual shortcut that appeared earlier in the project: allowing prey chemical energy to pay the electrolysis bill merely because both quantities can ultimately be expressed in joules. They represent different resource pathways inside the proposed organism and have to close in their appropriate ledgers.

### Series-current accounting

The later producer branches exposed another accounting issue. When two electrochemical or biological functions are opposite half-reactions of the same series circuit,

\[
I_{\rm anode}=I_{\rm cathode}
\]

The same current passes both sides of the circuit. It cannot be charged twice to the source simply because two different biological functions benefit from the complementary reactions.

This series-current rule becomes important in the producer architectures discussed later in the companion, particularly TC-11, and in understanding why some earlier T8-O accounting is retained only as historical or nonportable.

### Technical Trace — TC-05

**Primary CCID:** CC-B2-01  
**Project authority:** AP-CFINAL, AP-FZ  
**External package:** SP-B1-01  
**Current run:** SIM-EU-14  
**Historical/superseded:** SIM-EU-07 food-derived break-even/headroom fields  
**Prohibited stronger reading:** “biological electrolysis has been demonstrated under Europa conditions.”

---

# Part II — Building a Whole Organism

## TC-06 — Oxygen Demand, Respiration, and Gas Handling

Baseline Fulgoray is a heterotroph. Prey supplies reduced carbon, biological building material, nutrients, and conventional metabolic substrate. K1 electricity performs a different job: it supports the electrochemical production of oxygen and the associated electrical chemistry required for respiration.

Keeping those roles separate matters because the organism cannot be closed by comparing only total joules. The electrical source must satisfy the oxygen-production requirement, while the prey and material ledgers have to close independently.

### P0-A — biological oxygen-demand envelope

P0-A did not measure the respiration of a Fulgoray. No such organism exists to measure. Instead, it constructed an oxygen-demand envelope from terrestrial microbial reference measurements and used those values as model inputs.

The retained cases are:

- **Case A — HTCC7211 central:** approximately \(2.07\times10^{-17}\) to \(5.55\times10^{-17}\) mol O\(_2\) h\(^{-1}\) per biological-reference unit, with an uncertainty corridor of approximately \(1.73\times10^{-17}\) to \(7.27\times10^{-17}\).
- **Case B — RB2256 corridor:** approximately \(5.67\times10^{-16}\) to \(1.05\times10^{-15}\) mol O\(_2\) h\(^{-1}\), with a separate batch reference of \(1.4382\times10^{-15}\).
- **Case C — stress:** approximately \(1.8972\times10^{-15}\) mol O\(_2\) h\(^{-1}\).

These values are analogue-derived demand states, not measured Fulgoray respiration rates.

The corresponding stoichiometric electrical requirement is:

\[
I_{\rm required}=4F\dot n_{O_2}
\]

where \(F\) is the Faraday constant.

The project did not add an arbitrary maintenance multiplier merely to make the calculation conservative, and it did not invent a cold-temperature correction unsupported by evidence. The demand envelope is intended to remain traceable to the biological references from which it was constructed.

### Functional oxygen containment

The architecture eventually moved away from the idea that Fulgoray needs a large internal oxygen reservoir. The retained topology instead places production close to consumption:

\[
\text{OER microzone}
\rightarrow
\text{short O}_2\text{ path}
\rightarrow
\text{respiratory sink}
\]

SIM-EU-12 tested whether bulk oxygen transport becomes limiting at the minimum/reference demand scales. In the modeled states it did not. Even one adverse modeled corner retained diffusion capacity approximately 172 times demand, with a characteristic inventory time of about 23.85 s and diffusion time of about 0.415 s. A 10-\(\mu\)M reference state also remained hundreds of times above demand in that screen.

Those values are model consequences, not measurements of a biological compartment. Their significance is limited: the reference transport calculation did not force a large oxygen-storage organ.

Actual biological containment remains unresolved. A real organism would still need to keep oxygen where it is useful, limit exposure of incompatible chemistry, tolerate local gradients, and prevent oxidative damage.

### Hydrogen disposal

For the retained water-splitting topology, hydrogen is a cathodic coproduct. The minimum Fulgoray does not receive automatic food credit for that hydrogen simply because it is produced internally.

SIM-EU-12 therefore treated hydrogen primarily as a gas-disposal problem. The modeled vent-radius distribution remained microscopic across most tested states, but this result is again a consequence screen rather than a final anatomical prediction. It does not specify the number, geometry, material, or developmental origin of real gas-release structures.

Hydrogen can become ecologically interesting in later pathways, but reuse has to close its own carbon, nutrient, producer, retention, and transfer requirements.

### Biological oxygen-gradient analogues

Earth biology provides useful qualitative precedent for maintaining steep oxygen gradients. Known biological systems combine rapid local consumption, hydrated barriers, controlled permeability, geometry, and compartmentation to keep strongly different chemical conditions close together.

Gate D used such systems as **capability analogues**, not as direct anatomical templates for Europa. Their dimensions, organisms, membranes, chemistry, and transport properties are not imported as Fulgorax parameters.

The justified inference is therefore narrow: biology can maintain steep local oxygen gradients as a mechanism class. The actual Fulgoray containment and separator architecture remains unresolved.

### Autotoxicity remains a separate problem

Bulk diffusion closure does not solve the chemical hazards created by local oxygen production. Relevant unresolved burdens include reactive oxygen species, catalyst-side radicals, local oxidative damage, membrane and seal compatibility, pH and ionic gradients, and the protection of nearby chemistry that may require reducing or anaerobic conditions.

Gate D therefore did not produce an empirical containment pass. It showed that bulk gas transport need not be the limiting problem in the reference calculation while leaving the biological implementation and toxicity problem open.

### Technical Trace — TC-06

**Primary CCIDs:** CC-P0A-01, CC-D-01  
**Current `[SIM]`:** SIM-EU-01, SIM-EU-12  
**External package:** SP-P0A-01 plus generalized biological oxygen-gradient capability analogues  
**Unresolved:** containment, autotoxicity, and material implementation  
**Prohibited interpretation:** treating the reference demand envelope as measured Fulgoray respiration

---

## TC-07 — Eating in the Dark: Prey, Farming, and Sustainable Supply

Fulgoray is not a triboautotroph. K1 can provide an electrical service, but the baseline organism still requires reduced biological material and matter from outside itself. Ecology therefore enters the minimum-creature problem directly rather than appearing only after the organism has been designed.

### The permanent ecology firewall

A prey concentration is not the same thing as a sustainable food supply:

\[
\text{PREY DENSITY}
\neq
\text{PREY SUPPLY}
\]

A local environment can contain many cells while still failing to feed a consumer if those cells are not replenished quickly enough. Sustainable prey supply depends on concentration, flow, replenishment, depletion, capture cross-section, retention, ingestion, assimilation, and the hydrodynamic interference created by the feeding system itself.

This distinction prevents a static density measurement from being converted directly into a long-term feeding rate.

### Gate G — four ecological pathways

Gate G retained four conceptual routes:

1. **G1 — ambient microbial prey**
2. **G2 — waste-H\(_2\)-assisted farming**
3. **G3 — paid electrical farming**
4. **G4 — mechanotrophic ecology**

Only G1 is required for the baseline Fulgoray reference. The remaining pathways are alternatives or supplements rather than hidden assumptions needed to make the minimum organism close.

### Ambient prey and the D2 analogue

For one dense comparison regime, the project used an Earth diffuse-vent-like test class around:

\[
10^5\ \mathrm{cells\,mL^{-1}}
\]

This is the **D2 analogue regime**.

It is not a prediction of microbial abundance beneath Europa's ice. Its role is to ask a conditional question: if the local environment were comparably dense, would minimum-reference food throughput obviously fail?

Within the retained assumptions, that screen did not exclude closure. It did not establish a sustainable Europan prey field, a final feeding structure, or a particular capture strategy.

The result should therefore be read as **conditional compatibility at an Earth-analogue test regime**, not as evidence that Europa provides the required prey concentration.

### Waste hydrogen is not free food

Water splitting can produce hydrogen, which creates an obvious ecological possibility: hydrogen-consuming producers might use the coproduct and later become food for Fulgoray.

The project does not grant that loop for free.

A viable H\(_2\)-assisted producer still needs its own physiology, inorganic carbon, nutrients, biomass yield, retention, capture, assimilation, and ecological stability. Hydrogen solves only part of that chain.

The correct interpretation is therefore:

> **H\(_2\) is a coproduct and potential resource, not automatically food.**

A producer system can be investigated, but its output cannot be inserted into the prey ledger without paying the costs that create and deliver the biomass.

### Paid electrical farming

G3 is different because the organism deliberately allocates additional electrical current to supporting producer biomass rather than treating farming as a free consequence of the baseline oxygen circuit.

The accounting rule is:

\[
I_{\rm total}
=
I_{\rm baseline,O2}
+
I_{\rm farm}
\]

Electrical farming therefore increases source demand. It cannot reuse the baseline oxygen-production current as though the same current independently paid two unrelated processes.

The early G3 simulations, SIM-EU-22 and SIM-EU-23, remain valid as historical scaffolding for the topology in which they were run. They are not numerically portable into the final Fulgorad, Fulgoral, or Fulgoraz architectures, which reorganized the relationship between electrical service, carbon acquisition, and producer metabolism.

That topology firewall matters because an earlier simulation can remain internally correct while becoming inappropriate for a later architecture.

### Mechanotrophic ecology

Gate G also considered a more speculative route in which ecological productivity is supplied partly or indirectly by environmental mechanical energy through mechanotrophic organisms.

The project found no sufficiently strong empirical productivity law to give baseline Fulgoray numerical credit for that pathway. Mechanotrophy therefore remains an ecological possibility rather than a solved food source.

This does not establish that mechanotrophy is infeasible. It means the Europa minimum-creature calculation could not responsibly assume an organism-scale relation between fluid motion and biological productivity that had not been demonstrated or quantitatively modeled strongly enough for use.

### Technical Trace — TC-07

**Primary CCID:** CC-G-01  
**Current runs:** SIM-EU-18 through SIM-EU-21  
**Historical scaffolding:** SIM-EU-22 and SIM-EU-23  
**External package:** SP-G-01, with mixed citation readiness  
**Permanent firewall:** D2 is an Earth-analogue test regime, not a predicted Europa abundance

---

## TC-08 — Durability, Repair, Development, Reproduction, and Organization

A viable organism has to do more than make its chemistry work once. It must preserve enough functional structure to survive repeated operation, repair or replace damaged components, grow the machinery required for adult function, reproduce, and produce descendants that can construct the same system again.

These requirements brought Gate F, covering durability and repair, and Gate H, covering biological organization, into the whole-creature closure. Both ultimately received the same disposition:

> **UNRESOLVED-EMPIRICAL / DESK-SCIENCE COMPLETE**

The project found no desk-science contradiction that eliminated every admissible implementation, but it also lacked the empirical measurements needed for full closure.

### Gate F — durability

Gate F did not identify a universal K1-family durability failure. It also did not establish an empirical service life for assembled K1.

That distinction is essential:

\[
\text{C1 lifetime scenario}
\neq
\text{K1 empirical lifetime}
\]

The C1 lifetime sweep is a consequence map. It shows how other burdens change **if** particular lifetime states are assumed. It does not measure how long the organ actually lasts.

Potential failure modes include flexural fatigue, root or seam fatigue, seal failure, delamination, abrasion, biofouling, mineral deposition, catalyst degradation, oxidative damage, and progressive loss of the required contact geometry. No single favorable lifetime reported for a neighboring engineered material or biological structure was adopted as “the K1 lifetime,” because none directly measures the assembled organ.

This is a case where a broad literature can show that individual materials or functions are possible while still leaving the integrated lifetime unknown.

### Repair can matter as much as absolute lifetime

Short component lifetime does not necessarily kill an organism if damaged material can be replaced locally and affordably. Conversely, an apparently long-lived component can still be biologically expensive if repairing or reconstructing it requires too much specialized production.

For a replaceable region of mass \(M_R\) and service time \(T_{K1}\), the required replacement production rate is:

\[
\frac{M_R}{T_{K1}}
\]

If specialized biological production capacity is represented as \(q_R M_{\rm bio}\), a necessary repair relation is:

\[
q_R M_{\rm bio}
\ge
\frac{M_R}{T_{K1}}
\]

or equivalently:

\[
T_{K1,\min}
=
\frac{M_R}{q_R M_{\rm bio}}
\]

These equations are useful because they identify the quantities needed for closure: damaged mass, service life, biologically available production capacity, and repair locality. They do not provide those missing values.

A future empirical program therefore needs to measure not just how long K1 lasts, but **how it fails**. Local replaceable damage and whole-organ failure create very different biological burdens.

### Gate H — minimum biological organization

The organism already requires functions that cannot plausibly occupy one chemically homogeneous volume: oxygen-evolution and reduction chemistry, local oxygen management, redox routing, feeding and digestion, structural support, and the machinery needed to reproduce the architecture.

A chemically homogeneous unicell was therefore eliminated.

That result does **not** force multicellularity.

The retained organization ladder is:

- **H5-U** — compartmentalized unicellular-class architecture
- **H5-S** — syncytial or coenocytic bridge
- **H5-C** — minimally differentiated multicellular option, dominated at the minimum by lower-complexity alternatives where those remain admissible
- **H5-M** — stronger multicellular escalation if later constraints require it
- **H5-X** — parked higher-organization space

H5-U is the lowest-complexity class **not excluded** by the integrated analysis. It is not evidence that one ordinary cell is sufficient, nor does it specify final organelle structure, membrane count, nucleus-like organization, or developmental mechanism.

The distinction is important because “unicellular-class” here refers to a lineage-capable architecture with substantial internal compartmentation, not a chemically uniform microbe with all functions mixed together.

### Development and lineage closure

The correct object of analysis is the reproductive lineage, not only a finished adult.

Conceptually:

\[
P \rightarrow D \rightarrow A \rightarrow P'
\]

where propagule \(P\) passes through development \(D\), becomes adult \(A\), and eventually produces a new propagule \(P'\).

A viable adult architecture therefore does not close the lifecycle by itself. The developing organism must acquire or construct K1, containment, feeding structures, electrochemical machinery, repair systems, and whatever compartmentation the mature architecture requires.

The project explicitly rejects the shortcut:

\[
\text{IMMATURE PROPAGULE}
\neq
\text{FREE DEVELOPMENTAL INTERVAL}
\]

Development consumes matter and energy, and those costs cannot disappear merely because the adult has not yet begun normal operation.

Likewise,

\[
T_{K1}
\neq
T_{\rm generation}
\]

unless evidence establishes such a relation. A tribowhip does not automatically need to last for an entire generation if it can be repaired or replaced, and a long generation time does not establish a long K1 service life.

These distinctions leave development empirically unresolved, but they prevent the mature organism from receiving a free reproductive pathway.

### Technical Trace — TC-08

**Primary CCIDs:** CC-F-01, CC-H-01  
**Project authority:** AP-CFINAL, AP-NR, AP-FZ  
**External package:** SP-H-01 for capability analogues; detailed Gate-F component literature remains citation-limited at report level  
**New Gate-F or Gate-H `[SIM]`:** none  
**Main empirical gaps:** assembled K1 service life, failure locality, repair capacity, integrated cellular organization, and developmental provisioning

---
# Part III — How Large, and What Kind of Fulgorax?

## TC-09 — The Smallest Fulgoray We Could Defend

The minimum-creature campaign eventually abandoned the idea that “minimum” should mean the shortest tribowhip, the smallest body diameter, or the fewest appendages. Those quantities are downstream consequences of architecture, not definitions of biological minimality.

The final question became:

> **What is the lowest-complexity lineage-capable whole-organism family that is not excluded when all carried constraints are applied together?**

For Fulgoray / M0-HET, C-final closed with:

> **UNRESOLVED-EMPIRICAL / DESK-SCIENCE COMPLETE**

and retained the reference:

> **C8-U / H5-U CONDITIONAL REFERENCE FAMILY**

This result applies only to Fulgoray. It is not a minimum-size integration for Fulgorad, Fulgoral, or Fulgoraz.

### Why there is no scalar minimum

The surviving minimum family can be represented schematically as:

\[
\mathcal M_{\min}
=
\{C(D,S,U,O,T,R,F,L)\}
\]

where the admissible state depends on coupled requirements including biological demand, source performance, useful electrical transfer, oxygen routing, transport, repair, feeding, and lineage closure.

No single dimension controls all of those requirements. A shorter K1 element may reduce one burden while worsening another. A smaller body may reduce transport distance while leaving insufficient internal organization for incompatible chemistry. Reducing biomass may lower oxygen demand while also reducing repair capacity or material-processing capability.

C-final therefore did not earn a numerical value for:

- minimum body diameter;
- minimum K1 length;
- minimum K1 count;
- exact final cell count;
- final feeding anatomy;
- final service life;
- final useful-transfer efficiency.

Earlier values such as a 1.5-mm tribowhip, roughly 1,600 whips, a roughly 0.5–1-mm body core, and a roughly 5-mm whole-organism envelope are historical/reference values only. They are not current minimum anatomy.

The minimum result is therefore architectural rather than geometric.

### What did survive the integrated minimum analysis

Within the executed reference scope, several possible failure modes were tested without becoming universal kills:

- no universal source-side K1 mechanical contradiction was demonstrated;
- the required useful-transfer fraction could be mapped without inventing an interface efficiency;
- electrochemical operating requirements could be bounded;
- minimum/reference anchoring was not a modeled kill;
- bulk oxygen and hydrogen transport were not modeled kills;
- dense Earth-analogue prey throughput remained conditionally compatible;
- no universal durability contradiction was demonstrated;
- multicellularity was not forced.

Taken together, those results left one low-complexity architecture family unexcluded.

That wording matters. “Unexcluded” does not mean demonstrated, optimized, or likely. Several lines in the minimum architecture terminate in empirical unknowns, especially useful loaded K1 transfer, service life, repair, ecological supply, containment, and development.

The surviving minimum family is therefore a **conditional reference architecture**: the lowest-complexity integrated family the project could defend without silently filling the empirical gaps.

### Why H5-U matters

The retained H5-U organization class is often easy to misread.

It does not mean that an ordinary chemically homogeneous microbe can perform every Fulgoray function inside one undifferentiated cell. Gate H explicitly rejected that interpretation. H5-U instead represents a strongly compartmentalized unicellular-class architecture capable of maintaining multiple incompatible functional zones.

The important conclusion is:

> **Multicellularity was not forced by the current integrated constraints.**

That is weaker than saying “one cell is enough,” but scientifically more defensible.

A syncytial, coenocytic, or multicellular realization remains possible. Later empirical measurements could even make one of those higher-organization states necessary. C-final simply did not earn that escalation.

### What would move the minimum result

The current minimum cannot be sharpened into a geometric number until several missing relations are measured.

A lower useful-transfer efficiency would push source-area burden upward. Short K1 service life could increase replacement and repair demand. Poor prey replenishment could increase capture area or force a different metabolic architecture. More demanding oxygen-containment biology could require additional compartmentation. Developmental constraints could make a low-complexity adult impossible to reproduce reliably.

Conversely, favorable measurements could widen the admissible minimum family without establishing one uniquely preferred morphology.

That is why the correct current result is a conditional family rather than one final creature.

### Technical Trace — TC-09

**Primary CCID:** CC-CFINAL-01  
**Frozen reference:** C8-U / H5-U  
**Branch scope:** Fulgoray / M0-HET only  
**Integrated evidence status:** `[SPEC-INTEGRATED]`  
**Prohibited interpretations:** “one cell is enough,” “the minimum creature is X mm,” or “C-final proved the creature”

---

## TC-10 — How Large Could a Fulgorax Become?

![TC-03 — Maximum Size: When the Design Space Runs Out](../figures/TC03_MAXIMUM_SIZE_JOINT_ADMISSIBILITY_FINAL_2026-09-26.png)

*Figure TC-03 — Maximum size / joint admissibility. Conceptual admissibility regions, not quantitatively calculated curves. Morphology and modularity may shift the ranges. No numerical maximum and no unique first-failing constraint have been established.*

The maximum-size campaign began with an intuitive expectation: some version of square-cube scaling would eventually become the dominant limit. Larger organisms tend to carry increasing structural, transport, and mechanical burdens, so it was reasonable to expect a relatively simple scaling failure.

The integrated result was more complicated.

MS11 closed as:

> **UNRESOLVED-EMPIRICAL / DESK-SCIENCE COMPLETE**

and retained four explicit negative conclusions:

1. **No numerical maximum was earned.**
2. **No unlimited-size claim was earned.**
3. **No unique first failure was earned.**
4. **No later M3 branch demonstrated a larger maximum than Fulgoray / M0.**

The project therefore does not contain an answer of the form “Fulgorax can reach X centimeters” or “branch Y grows larger than branch Z.” The current maximum result is a structure for identifying where a branch stops remaining jointly admissible.

### Maximum size as a joint-admissibility boundary

For branch \(b\) and requirement \(j\), the project uses a generic capacity ratio:

\[
\mathcal C_{j,b}
=
\frac{\text{available capacity}}
{\text{required capacity}}
\]

A state remains admissible only if some authorized realization satisfies all mandatory constraints simultaneously:

\[
\exists X_b:
\bigwedge_j \mathcal C_{j,b}(X_b)\ge1
\]

Along a chosen scaling coordinate \(\lambda\), the maximum is conceptually:

\[
\lambda_{\max}
=
\sup
\left\{
\lambda:
\text{all mandatory constraints remain jointly admissible}
\right\}
\]

The point of this formulation is that the first failed constraint cannot be identified independently of the morphology and architecture being scaled.

The scaling coordinate also does not have to be body diameter. Depending on the organism, scaling may involve biomass, footprint, projected area, K1 area or count, radial extent, thickness, branch length, number of modules, or throughput.

A sessile branching organism does not have to enlarge in the same way as an isometric animal.

### Why square-cube scaling remains important but is not decisive

Square-cube reasoning still matters inside individual problems. As size increases, drag, bending moment, attachment burden, transport distance, support requirements, and repair costs can all scale unfavorably.

But the organism is not required to remain geometrically similar as it grows.

Authorized responses include:

- flattening;
- branching;
- broad thin morphologies;
- distributed K1;
- distributed gas handling;
- modular feeding;
- repeated producer modules;
- syncytial or multicellular escalation;
- enlarged attachment footprints.

These responses can postpone a local constraint, but they are not free solutions. A wider footprint may improve anchoring while increasing material cost. More branching can increase functional area while increasing drag, transport, and repair burden. Distributed K1 may reduce some local bottlenecks while requiring more routing and support infrastructure.

Morphology is therefore part of the solution space, not a loophole that removes scaling limits.

### The shared K/A/R candidate backbone

Across all four final branches, the strongest recurring structural candidate is:

\[
\{K,A,R\}
\]

where:

- **K** = K1 deployment, structural support, source performance, and useful electrical service;
- **A** = anchoring force and bending moment in the same physical state used for source generation;
- **R** = empirical service life plus sustainable repair and replacement.

The project describes this set as **structurally implicated** rather than statistically “most likely.” No probability distribution over first-failure modes was established.

The importance of K/A/R is that these burdens recur regardless of which metabolic branch is chosen. All branches still need a generator, must survive the same mechanical environment, and must maintain the relevant structures over time.

Branch-specific biology then adds additional constraints.

### Branch-specific scaling registries

The retained branch registries are:

For Fulgoray:

\[
\{P,A,K,R\}
\]

For Fulgorad:

\[
\{P_D,A_D,K_D,R_D,DH\}
\]

For Fulgoral:

\[
\{A,K,R,Z,DH\}
\]

For Fulgoraz:

\[
\{A,K,R,Z,HS,Network,Transfer\}
\]

These are compact labels for the constraints that must remain jointly admissible as each branch scales.

The branch-specific terms represent different ways the organism can fail. Fulgoray retains external prey supply \(P\). Fulgorad adds direct-host electrical burden \(DH\). Fulgoral adds resource closure \(Z\) and direct-host producer interfaces. Fulgoraz replaces part of that topology with internal symbiont service \(HS\), network burden, and metabolite transfer.

No branch has been solved to a numerical terminal crossing.

### Why the final maximum-size simulation was not run

A sufficiently large solver could have been constructed by assigning distributions to the unknown K1 mechanics, service life, repair capacity, feeding performance, producer current, symbiont-network properties, and other unresolved parameters.

That would have produced numbers.

It would not have produced stronger science.

The project therefore made an explicit no-run decision at MS9 rather than filling the model with arbitrary distributions and treating the resulting maximum as evidence.

This is an important distinction in the Technical Companion: a missing simulation is not necessarily incomplete work. In this case, not running the simulation was the controlled scientific result because the unresolved inputs were too important for the output to carry the authority the calculation would appear to have.

### EF-MS1 — the next scaling experiment

The highest-priority maximum-size experiment is EF-MS1:

> **Measure electrical source behavior and force/moment in the same coherent K1 array across geometry, spacing, density, and flow.**

This requirement exists because the electrical benefit and mechanical burden of K1 must be measured in the same physical configuration. The project cannot responsibly combine source performance from one array geometry with anchoring loads from another and call the result one organism.

EF-MS1 is downstream of EF-1. There is little reason to characterize large-array scaling in detail before the basic K1 mechanism has demonstrated reproducible useful loaded transfer and reset.

### What the maximum-size result actually says

The final maximum-size conclusion is narrow:

> **Forms larger than the conditional minimum remain unexcluded, but no enlargement factor has been earned.**

The project has a finite conceptual boundary structure because real constraints eventually have to close simultaneously. What remains unknown is where that boundary lies and which empirical requirement crosses first in any particular branch and morphology.

This leaves square-cube scaling where it belongs: as an important contributor to several burdens, but not as a demonstrated single master limit.

The actual maximum-size problem is one of coupled mechanical, electrical, ecological, material, and biological closure.

### Technical Trace — TC-10

**Primary CCIDs:** CC-MAXDEF-01, CC-MS11-01  
**Project authority:** AP-MS11, AP-FZ, AP-NR  
**Future models:** SIM-FUT-01 / SIM-FUT-02 remain S0 and were not executed  
**Prohibited interpretations:** numerical maximum, unlimited size, unique first failure, or statistical ranking of K/A/R

---

## TC-11 — The Four Europa Fulgorax Forms

![TC-04 — Four Ways to Build a Europa Fulgorax](../figures/TC04_FOUR_FULGORAX_FORMS_FINAL_2026-09-26.png)

*Figure TC-04 — Four Fulgorax forms. Fulgoray, Fulgorad, Fulgoral, and Fulgoraz are alternative functional architectures, not an evolutionary sequence, sophistication ladder, species reconstruction, or size ranking. No creature morphology is implied by the comparison.*

The maximum-size campaign did more than ask how large the original organism could become. It forced the project to separate the different roles that “food” performs.

Food can supply reducing power, metabolic energy, carbon, nitrogen, phosphorus, sulfur, trace elements, and structural precursors. Electricity can replace some energetic or redox functions in some architectures, but it cannot replace matter simply by supplying more power. The four final Europa forms therefore differ mainly in **carbon source, electrical role, and the location of producer metabolism**. They are alternative architectures, not stages in a progression.

### TC-11.1 — Fulgoray (M0-HET)

Fulgoray is the best-closed reference architecture and the only branch with a completed C-final minimum integration. Its simplified division of labor is:

\[
\text{prey}
\rightarrow
\text{reduced carbon + matter}
\]

\[
\text{K1 electricity}
\rightarrow
\text{O}_2\text{ production}
\rightarrow
\text{respiration}
\]

Fulgoray is therefore fundamentally heterotrophic. Electrical generation does not remove its dependence on external reduced biological material.

Its maximum-size registry is:

\[
\{P,A,K,R\}
\]

where the branch-specific vulnerability \(P\) represents external prey supply. That term is not reducible to prey concentration alone; sustainable closure depends on the interaction among concentration, flow, capture, replenishment, depletion, and the same morphology that supports K1 and anchoring.

Fulgoray remains the reference branch because it has the strongest integrated closure, not because it is assumed to be evolutionarily primitive or generally superior.

### TC-11.2 — Fulgorad (M3-Dmix)

Fulgorad remains a consumer, but electricity takes over more of the energetic burden. The architecture uses electrical service to reduce some respiratory or reducing-equivalent demand so that a larger fraction of captured prey carbon can be retained for biomass and construction rather than oxidized.

That does not make the organism matter-independent. A residual prey floor remains:

\[
r_P \ge r_{P,\mathrm{matter}} > 0
\]

because carbon, nutrients, and structural material still have to come from somewhere.

A simplified representation of prey relief is:

\[
r_P(s)
=
\frac{\dot M_{\rm prey,Dmix}}
{\dot M_{\rm prey,M0}}
\]

while the corresponding electrical burden is:

\[
\kappa_I(s)
=
\frac{I_{\rm req,Dmix}}
{I_{\rm req,M0}}
\]

A prey/anchor sub-envelope may improve where:

\[
r_P\kappa_I < 1
\]

but that inequality does not prove that the entire organism gains a larger maximum size. It only identifies a region where reduced prey burden may outweigh some of the added electrical cost.

The future empirical requirement is one **coherent state trajectory**:

\[
s\mapsto
\{r_P(s),\kappa_I(s),I_{\rm subsidy}(s),V_{DH}(s),j_{DH}(s)\}
\]

The project may not take the strongest prey reduction from one state and combine it with the smallest electrical burden from a different, incompatible state. The biological and electrical terms have to describe the same organism state.

Fulgorad therefore provides a conditional way to reduce a prey/fuel ceiling, but it does so by adding direct-host electrical demand and additional K1 burden. No larger maximum than Fulgoray has been demonstrated.

### TC-11.3 — Fulgoral (M3-DA-U)

Fulgoral is the **direct host producer**. Instead of relying primarily on external biological prey for carbon, the host uses K1-derived electrical service to support inorganic carbon fixation directly.

Its conceptual chain is:

\[
K1
\rightarrow
\text{host electrical bioenergetics}
\rightarrow
\text{CO}_2/\text{DIC fixation}
\rightarrow
\text{host biomass}
\]

This can remove ambient prey as the main **fuel/carbon** ceiling, but it does not remove the organism's need for matter.

At the stoichiometric level, the minimum carbon-reduction current floor is:

\[
I_{\rm fix,min}=4F\dot n_C
\]

The actual producer burden is represented as:

\[
I_{\rm producer}
=
\Gamma_{\rm prod}(4F\dot n_C)
\]

where \(\Gamma_{\rm prod}\) remains unresolved. No terrestrial electrotroph supplies one universal value that can simply be inserted into the Europa architecture.

External matter demand persists and can be represented schematically as:

\[
\dot n_{z,\rm ext}
=
\nu_z
[\dot M_G+(1-r_z)\dot M_T+\dot M_{\rm export}]
\]

The governing firewall is:

\[
\text{ENERGY AUTONOMY}
\neq
\text{MATTER AUTONOMY}
\]

A host that can make its own reduced carbon still requires elements, minerals, replacement material, and whatever external resources cannot be internally recycled with perfect efficiency.

Fulgoral also introduces a feedback dependency:

\[
K\rightarrow R\rightarrow Z\rightarrow I\rightarrow K
\]

In words, K1 performance affects available resources; resources affect repair and material closure; those influence producer demand and current requirement; the current requirement feeds back into K1 burden.

The dependency is real as an accounting topology. The project has not computed a loop gain, runaway condition, or stable fixed point.

### TC-11.4 — Fulgoraz (M3-IS(O))

Fulgoraz moves producer metabolism into persistent internal symbionts.

Its conceptual chain is:

\[
K1
\rightarrow
HS
\rightarrow
Network
\rightarrow
Symbiont
\rightarrow
Transfer
\rightarrow
Host
\]

The internal producer system is not intended as “livestock in a gut.” The closer analogy is a persistent metabolic organ composed of symbiotic producer cells connected to host-controlled electrical, chemical, and material infrastructure.

The preferred transfer concept is continuous:

\[
e^-
\rightarrow
\text{symbiont}
\rightarrow
\text{reduced metabolite}
\rightarrow
\text{host}
\]

rather than repeatedly growing, killing, and digesting the symbionts. No exact transferred metabolite or symbiont lineage is frozen.

Fulgoraz also requires strict modularity controls. Total current remains conserved:

\[
\sum_m I_m=I_{\rm total}
\]

and several tempting shortcuts are prohibited:

\[
\text{INTERFACE SUBDIVISION}
\neq
\text{INTERFACE CAPACITY INCREASE}
\]

\[
\text{DISTRIBUTED SYMBIONTS}
\neq
\text{DISTRIBUTED INFRASTRUCTURE}
\]

\[
\text{LOCAL NETWORK CLOSURE}
\neq
\text{SHARED-BACKBONE CLOSURE}
\]

Breaking a producer system into many modules does not automatically increase total interface capacity, and distributing producer cells does not remove the shared costs of conductors, nutrients, oxygen control, metabolite return, repair, or regulation.

Fulgoraz therefore does not automatically outperform Fulgoral. Before invoking internal symbionts as a unique rescue, the project requires Fulgoral to exhaust legitimate host-only interface modularity through the **DH-MOD** pathway.

### T8-O and the series-current correction

An earlier producer architecture, M3-O(+H\(_2\)), received a large formal computation: T8-O / SIM-EU-24, containing 2,192,832 decision rows and passing 15/15 QA checks.

That run remains valid in the topology for which it was constructed.

It is not numerically portable to the final producer branches.

The permanent rule is:

> **OLD `[SIM]` AUTHORITY ENDS AT THE TOPOLOGY BOUNDARY.**

The circuit-level reason is:

\[
I_{\rm anode}=I_{\rm cathode}
\]

for a single series circuit. One current cannot be independently charged twice simply because its two half-reactions support different biological services.

The T8-O computation is therefore not discarded as bad work. It remains historical/nonportable evidence for the architecture it actually modeled.

### Four-form summary

- **Fulgoray:** consumes external biological prey; electricity chiefly supplies oxygen service.
- **Fulgorad:** remains dependent on external matter; electrical subsidy reduces some prey-oxidation burden.
- **Fulgoral:** the host directly fixes inorganic carbon using electrical bioenergetics.
- **Fulgoraz:** persistent internal symbionts perform producer metabolism and transfer products to the host.

The four forms are alternatives rather than rankings. The project did not establish an evolutionary sequence, a sophistication ladder, or a maximum-size ordering among them.

Direct controlled physiology would be required to distinguish these architectures experimentally. Remote chemistry alone would generally be insufficient because many of the relevant products and reactants are shared with ordinary biological and abiotic processes.

### Technical Trace — TC-11

**Primary CCIDs:** CC-M0-01, CC-DMIX-01, CC-DAU-01, CC-ISO-01, CC-T8O-01  
**Project authority:** AP-MS11, AP-BC, AP-FZ  
**No branch ranking:** true  
**No demonstrated M3 \(>\) M0 maximum:** true  
**Historical run:** SIM-EU-24, valid within original topology and nonportable to the final branches

---

## TC-12 — What Nature Already Does — and What It Does Not

Speculative organism design becomes misleading when individual mechanism precedents are stacked until the collection begins to look like precedent for the integrated organism.

The Technical Companion therefore enforces a permanent distinction:

\[
\boxed{
\text{MECHANISM ANALOGUE}
\neq
\text{INTEGRATED ARCHITECTURE}
}
\]

Earth biology, bioelectrochemistry, and microbial ecology demonstrate many component capabilities relevant to the final Fulgorax branches. None demonstrates Fulgorax as an integrated organism.

### Electrode-associated electron uptake and carbon assimilation

Several primary studies provide relevant precedent for biological use of electrode-supplied electrons:

- **[Nevin et al. (2010)](https://doi.org/10.1128/mBio.00103-10)** — electrode-fed acetogenic CO\(_2\) reduction.
- **[Bose et al. (2014)](https://doi.org/10.1038/ncomms4391)** — electrode electron uptake associated with CO\(_2\) assimilation in *Rhodopseudomonas palustris* TIE-1.
- **[Ranaivoarisoa et al. (2019)](https://doi.org/10.1038/s41467-019-09377-6)** — stronger coupling between extracellular electron uptake and CO\(_2\) fixation.
- **[Ishii et al. (2015)](https://doi.org/10.3389/fmicb.2015.00994)** — nonphotosynthetic electrolithoautotrophic enrichment.

Together these studies establish that electrical input can participate in microbial carbon metabolism. They do not establish a K1-powered host producer on Europa.

Their role in the project is therefore to support a **mechanism class**: biological systems can, under some conditions, incorporate externally supplied electrical reducing power into carbon metabolism.

### Direct versus mediated electrotrophy

Apparent electrode-driven metabolism does not necessarily mean electrons pass directly from an electrode into a biological electron-transport chain. Hydrogen, formate, or other intermediates may mediate the process.

[Tremblay et al. (2019)](https://doi.org/10.3390/catal9020166) is retained specifically to protect the distinction:

\[
\text{APPARENT ELECTROTROPHY}
\neq
\text{PROVEN DIRECT MOLECULAR ELECTRON UPTAKE}
\]

This matters for Fulgoral because the electron-entry mechanism affects interface current density, required voltage, physical hardware, biochemical routing, and the amount of host tissue needed to support the process.

A mediated process could still be useful, but it would be a different architecture with different material and scaling costs.

### Long-range biological conduction

Biological systems also provide strong precedent for long-range electrical transport. [Summers et al. (2010)](https://doi.org/10.1126/science.1196526) demonstrated interspecies electrical interaction in conductive microbial aggregates, while [Pfeffer et al. (2012)](https://doi.org/10.1038/nature11586) demonstrated centimetre-scale electron transport in cable bacteria.

These observations show that biological conduction over distances much larger than a single molecular complex is possible.

They do not establish the Fulgoraz electrotrophosome, and they do not show that adding conductive biological structures automatically increases K1 collection or producer-interface capacity. Conductivity can help route electrons without creating new source current.

### Internal autotrophic symbiosis

Persistent internal producer symbioses also have strong biological precedent.

[Felbeck (1981)](https://doi.org/10.1126/science.213.4505.336) demonstrated chemoautotrophic carbon fixation in *Riftia* symbiosis. [Bright, Keckeis & Fisher (2000)](https://doi.org/10.1007/s002270050722) subsequently traced newly fixed symbiont carbon into host tissues. These systems support the plausibility of internal producer cells supplying fixed carbon to a larger host.

They do not demonstrate **host-to-symbiont electrical powering**.

That missing direction of service is central to Fulgoraz. Existing symbioses show that a host can maintain internal producers and receive products from them; they do not establish the K1 → electrical network → symbiont part of the proposed architecture.

### Biological electrical organs, reset, and homeostasis

Living systems can build specialized membranes, maintain electrochemical gradients, generate electrical signals, compartmentalize incompatible chemistry, and repair electrically active tissues.

Those capabilities are relevant analogues for K1 control, buffering, countercharge management, and reset.

They do not specify the K1 circuit.

The project therefore uses electrical organs and other biological electrochemical systems as evidence that living material can perform sophisticated charge management, not as evidence that the specific hydrated contact-separation generator has already been solved by evolution.

### Hydrothermal electrical activity is not tribotrophy

Natural conductive minerals and hydrothermal electrochemical gradients can generate electrical currents. Electrotrophic organisms can consume environmental electrons.

Neither phenomenon is tribotrophy.

\[
\text{ELECTRICAL ACTIVITY}
\neq
\text{TRIBOELECTRIC LIFE}
\]

\[
\text{ELECTROTROPHY}
\neq
\text{TRIBOTROPHY}
\]

The defining source pathway for tribotrophy is environmental mechanical work acting on a biologically organized contact-separation structure, with the resulting electrical output delivered into a biological function.

This distinction is especially important in hydrothermal settings because electrical phenomena can occur there for many abiotic and biological reasons that have nothing to do with triboelectric energy harvesting.

### Evidence ladder

The project uses a simple hierarchy to keep precedent from being overinterpreted:

1. **mechanism class exists**;
2. **relevant analogue exists**;
3. **coupled subsystem exists**;
4. **integrated Fulgorax architecture exists**.

The literature provides many Level-1 and Level-2 precedents, a much thinner set of Level-3 coupled subsystems, and no Level-4 empirical Fulgorax.

That is why the final organism architectures remain `[SPEC-INTEGRATED]`.

The inverse inference is also prohibited. Failure to find an Earth organism that already integrates every Fulgorax function does not prove that such integration is impossible. Absence of an integrated analogue is an unresolved evidence gap, not a demonstrated biological contradiction.

### Technical Trace — TC-12

**Primary CCIDs:** analogue support associated with CC-DMIX-01, CC-DAU-01, and CC-ISO-01  
**Primary-source / cross-referenced packages:** SP-EF1-01, SP-H-01, SP-MS5-01, SP-FC-01, each only within normalized applicability  
**Recovered FC1 register:** Nevin, Bose, Ranaivoarisoa, Ishii, Tremblay, Summers, Pfeffer, Felbeck, Bright  
**Permanent inference rule:** mechanism analogue does not equal integrated architecture

---
# Part IV — Detection, Earth Experiments, and the Research Roadmap

## TC-13 — Chemistry, Biosignatures, and the Direct Test

![TC-05 — How Would We Know?](../figures/TC05_HOW_WOULD_WE_KNOW_CAUSAL_CHAIN_FINAL_2026-09-26.png)

*Figure TC-05 — How Would We Know? The full causal chain is more diagnostic than H₂, O₂, organics, or current alone, but it is not established as uniquely biological or proof of tribotrophy. It is a conditional direct-detection architecture, not an observed Europa biosignature.*

A speculative organism is not scientifically complete once its anatomy and metabolism have been described. If it exists, it must also interact with its environment: consuming resources, moving electrons, releasing products, shedding material, and changing local chemistry.

That creates a strong temptation to take any expected product—hydrogen, oxygen, carbon dioxide, organics, electrical activity—and call it a biosignature. The forward-chemistry phase was designed specifically to prevent that shortcut.

For each candidate signal, the project followed the chain:

\[
\boxed{
\text{organism mechanism}
\rightarrow
\text{product}
\rightarrow
\text{flux}
\rightarrow
\text{environmental fate}
\rightarrow
\text{confounders}
\rightarrow
\text{detectability}
\rightarrow
\text{falsification}
}
\]

A compound produced inside the organism is not necessarily exported. An exported compound is not necessarily stable. A persistent compound is not necessarily detectable. A detectable signal is not necessarily biological, and a biological signal is not necessarily triboic.

That sequence removed most of the seemingly obvious signatures. The final forward-chemistry disposition is:

> **FC — UNRESOLVED-EMPIRICAL / DESK-SCIENCE COMPLETE**

with the central conclusion:

> **No chemistry-only triboic-specific biosignature has been earned.**

### Hydrogen — direct product, weak signature

For baseline Fulgoray, the retained OER/HER topology produces hydrogen on the cathodic side. The ideal stoichiometric relation is:

\[
2H_2\ \text{per}\ O_2
\]

Using the already-retained P0-A oxygen-demand family, the forward-chemistry work mapped the corresponding hydrogen production to approximately:

\[
3.47\times10^{-17}
\text{ to }
3.79\times10^{-15}
\ \mathrm{mol\ H_2\ h^{-1}}
\]

or roughly:

\[
5.8\times10^3
\text{ to }
6.35\times10^5
\ H_2\ \text{molecules s}^{-1}
\]

per P0-A biological-reference unit.

These numbers are useful for chemical bookkeeping. They are not measured Fulgorax fluxes, whole-organism fluxes, population fluxes, regional Europa source strengths, or new `[SIM]` results.

Hydrogen also has strong abiotic and ordinary biological production routes, including water-rock reactions. The retained classification is therefore:

> **Fulgoray H\(_2\) = NON-SIGNATURE / CONTEXTUAL REDOX TRACER ONLY**

Hydrogen could still help characterize local redox conditions or support ecological hypotheses. It simply does not identify tribotrophy.

### Carbon dioxide and dissolved inorganic carbon

Baseline Fulgoray oxidizes reduced prey carbon, so some carbon may return to the environment as CO\(_2\) or dissolved inorganic carbon.

The project did not assign a universal respiratory quotient:

\[
n_{CO_2}
=
R_{CO_2/O_2}n_{O_2}
\]

because \(R_{CO_2/O_2}\) remains unresolved for the hypothetical organism. Carbonate buffering, mineral reactions, mixing, ordinary respiration, and autotrophy all provide additional confounders.

The retained classification is:

> **Fulgoray CO\(_2\)/DIC = NON-SIGNATURE / CONTEXTUAL CARBON-CYCLE VARIABLE**

### Producer oxygen

Fulgoral and Fulgoraz may produce oxygen while fixing inorganic carbon, but environmental export requires net production to exceed all local sinks:

\[
J_{O_2,\mathrm{OER}}
>
J_{O_2,\mathrm{ORR}}
+
J_{O_2,\mathrm{resp}}
+
J_{O_2,\mathrm{other}}
\]

This is a threshold relation, not evidence that any real producer branch crosses that threshold. No achieved producer-oxygen flux has been assigned. Radiolysis, geochemistry, and ordinary biology also provide oxygen confounders on planetary and local scales.

Even a coupled pattern of oxygen production and DIC uptake remains non-specific:

\[
O_2+\text{DIC uptake}
=
\text{NON-SPECIFIC MULTIPROCESS PATTERN / CONTEXT ONLY}
\]

The pattern may be interesting, but it cannot uniquely identify tribotrophy.

### Fulgorad has no unique environmental product

Fulgorad differs mainly in **carbon partitioning**, not in producing a uniquely diagnostic molecule. Electrical subsidy may reduce the fraction of prey carbon oxidized at matched growth, but natural organisms already span wide ranges of carbon-use efficiency.

Fulgorad therefore has no earned remote environmental biosignature. Its distinction is better approached as a future **controlled physiology** problem in which carbon allocation and electrical subsidy can be measured together.

### Debris is not enough

Ordinary biomass, membrane fragments, structural polymers, seal material, catalyst supports, and damaged K1 tissue would all be strongly confounded by ordinary biological or abiotic material. Generic turnover organics are therefore non-signatures.

A recovered biological structure becomes more interesting only if multiple functional properties remain associated, such as organized morphology, differentiated material regions, repeatable contact-separation electrical behavior, evidence of biological construction or repair, and a function inconsistent with ordinary tissue or conductive mineral debris.

The retained classification is:

> **CONDITIONAL FUNCTIONAL-MATERIAL DIRECT-DETECTION CANDIDATE / DIRECT ACCESS REQUIRED**

No actual K1 sample exists, and the environmental transport of an intact functional K1-like structure has not been demonstrated.

### The strongest detection concept is causal

The strongest surviving route is not a molecule. It is a mechanism-level causal test.

A serious tribotrophy test requires, at minimum:

1. a biological or strongly biologically organized structure;
2. measured local mechanical forcing;
3. an identifiable motion/contact/separation state;
4. repeatable electrical output synchronized with that state;
5. response under a controlled electrical load;
6. colocated chemistry consistent with real biological or electrochemical service;
7. electrical response that changes when motion/contact is perturbed and returns when restored;
8. mineral, dead-material, sampling-artifact, and ordinary-electrobiology controls that fail to reproduce the complete chain.

Conceptually:

\[
\boxed{
\text{flow}
\rightarrow
\text{K1 motion/contact}
\rightarrow
\text{charge generation}
\rightarrow
\text{useful loaded electrical service}
\rightarrow
\text{local chemistry}
}
\]

The individual observations are not unique. The full causal conjunction is much harder to reproduce accidentally.

### Why remote chemistry cannot directly demonstrate tribotrophy

A chemical product generated near Europa's seafloor would have to survive a long transport chain before reaching an accessible surface, plume, or exosphere reservoir. Schematically:

> seafloor → vent habitat → hydrothermal plume → deep ocean  
> deep ocean → ice-ocean interface → ice shell → sampled surface/exosphere/plume reservoir

The project deliberately did not invent transfer coefficients through this sequence. Current or near-term remote measurements can provide valuable environmental and provenance information, but they cannot directly establish:

\[
\text{biological structure}
\rightarrow
\text{contact/separation}
\rightarrow
\text{load-bearing electrical generation}
\]

No Europa transport/detectability `[SIM]` is currently admitted.

Failure to identify a unique remote biosignature is also **not** evidence against the physical feasibility of the organism. Detectability and viability are separate questions.

### Technical Trace — TC-13

**Primary CCIDs:** CC-FC-H2-01, CC-FC-O2-01, CC-FC-DIC-01, CC-FC-K1-01, CC-FC-CAUSAL-01, CC-FC7-01  
**Project authority:** AP-FC7, AP-NR, AP-FZ  
**New FC `[SIM]`:** none  
**Strongest detection route:** causal mechanism test rather than chemistry-only signature

---

## TC-14 — The Earth Diffuse-Vent Experimental Program

![TC-06 — Reanimating the Vent Subsurface](../figures/TC06_VENT_SUBSURFACE_REANIMATION_FINAL_2026-09-26.png)

*Figure TC-06 — Reanimating the Vent Subsurface. Proposed flow-through reanimation experiment, not an experimental result. Revival is not assumed, and a first-ever novelty claim is not earned.*

Europa is extremely difficult to access. Earth's ocean floor is difficult as well, but it is experimentally reachable.

That makes terrestrial hydrothermal and subseafloor environments useful for testing parts of the broader Triboic Life hypothesis. The purpose is not to assume that Earth contains Fulgorax. It is to use accessible environments in which sustained fluid motion, reduced chemistry, anoxia, mineral surfaces, microbial communities, and unusual physiological strategies can be studied directly.

The program is deliberately staged. A revived microorganism from a vent or subseafloor core would be biologically interesting, but it would not automatically be evidence for tribotrophy.

### EARTH-A — prior art and sample feasibility

Before making any novelty claim, the first step is to determine how closely existing experiments match the proposed design.

The targeted project review found related precedents but did not establish an exact match. The approved wording is:

> **Targeted review found close precedents, but no exact match was established; a first-ever claim is not earned without a comprehensive literature, protocol, cruise-report, repository, and patent review.**

The scientific value of the experiment does not depend on being first.

Sample history is equally important. Archived material should retain, as far as possible, information about collection location, sample type, preservation, storage, available volume, contamination history, freezing, decompression, chain of custody, and likely viability.

A failure to recover life from badly preserved material has very different meaning from a failure using fresh pressure-retained samples.

### EARTH-B — archived-core reanimation pilot

The proposed pilot is straightforward:

> **Obtain suitable archived diffuse-hydrothermal or subseafloor core material, run anoxic seawater through it continuously for weeks to months, and monitor for reproducible biological revival or growth.**

The treatment matrix should include several deliberately different arms rather than one highly optimized condition.

#### Native or site-like arm

Approximate source chemistry as closely as the archive and sample history permit. This arm asks whether organisms recover under conditions intended to resemble their original habitat.

#### Nutrient-rich arm

Use nutrient-rich anoxic seawater to maximize broad revival opportunity. This is not intended as a perfect ecological reconstruction. Its purpose is to ask whether recoverable biological potential remains in the sample.

#### Vent-metabolism-enriched arm

Where justified by the source environment, add reduced inorganic substrates or other chemistry relevant to known hydrothermal metabolic classes.

#### Flow variation

Flow should itself be varied because it can alter nutrient delivery, waste removal, surface exchange, physical disturbance, attachment, and material transport. The point is not to assume that flow is an energy source, but to determine whether it changes recovery or growth.

#### Controls and observations

At minimum, the program should include sterile controls, non-vent controls, preserved baseline subsamples, contamination controls, and procedural blanks where appropriate.

Useful measurements can include microscopy, cell counts, biofilm or filament formation, resting-stage emergence, DNA/RNA, local chemistry, and unusual organized structures.

### Interpreting a positive result

The primary positive result is simply:

> **reproducible biological growth or revival above controls**

That could indicate dormant cells, resistant stages, spores, suppressed populations, or organisms that were not obvious in the initial material.

It would justify further work, but it would not identify tribotrophy:

\[
\boxed{
\text{REVIVAL}
\neq
\text{TRIBOTROPHY}
}
\]

A positive culture becomes relevant to Triboic Life only if later work identifies an unusual mechanical-electrical-biological mechanism.

### Interpreting a negative result

A negative archived-core pilot has much weaker meaning.

Failure to revive biology could reflect true absence, but it could also result from collection damage, decompression, freezing, storage history, oxygen exposure, incorrect medium, missing ecological partners, missing minerals, insufficient duration, or continued dormancy.

Therefore:

\[
\boxed{
\text{NEGATIVE ARCHIVED-CORE PILOT}
\neq
\text{NO DEEP LIFE}
}
\]

A negative archived-core result has weak exclusion power unless preservation and cultivation conditions are unusually well controlled.

### EARTH-C — fresh and pressure-retained follow-up

If archived material produces a promising result, or if preservation history makes interpretation impossible, the next stage should move toward fresh material where feasible.

Important improvements include:

- fresh core or fractured subsurface material;
- pressure-retaining collection;
- faithful temperature;
- preserved anoxia;
- matched chemistry;
- controlled flow.

Fresh or pressure-retained sampling improves both positive and negative inference because the experiment more closely represents the ecological state being tested.

### EARTH-D — causal tribotrophy experiment

If an unusual organism or structure is associated with flow, the next step is not to label it triboic. The experiment must test the defining causal pathway.

A strong setup combines:

- high-resolution imaging;
- local flow measurement;
- motion tracking;
- contact/separation-state tracking;
- voltage and current waveforms;
- a controlled external load;
- O\(_2\), H\(_2\), redox, pH, and DIC measurements where relevant;
- material analysis;
- motion/contact perturbation;
- mineral-current controls;
- dead or sterilized material controls.

The core test is:

\[
\text{motion/contact ON}
\rightarrow
\text{electrical response}
\]

\[
\text{motion/contact reduced}
\rightarrow
\text{electrical response changes}
\]

\[
\text{motion/contact restored}
\rightarrow
\text{electrical response returns}
\]

The next question is whether the colocated chemistry changes consistently with the electrical service.

A biological conductor sitting on an electrically active mineral is not enough. An electrotroph consuming mineral electrons is not enough. A strong tribotrophy claim requires the combined package:

\[
\boxed{
\text{biological structure}
+
\text{motion/contact}
+
\text{loaded electrical response}
+
\text{perturbation}
+
\text{local chemistry}
+
\text{controls}
}
\]

### Why dead-material controls are unusually important

A dead biological structure can retain passive triboelectric properties. That makes living-versus-dead comparisons especially informative.

Passive charge generation may continue after death, while active reset, repair, ion return, regulation, and redox recovery may disappear. The comparison could therefore help distinguish a merely triboelectric biological material from a living tribotrophic system.

### EARTH-E — Earth is not Europa

Even discovery of a genuine terrestrial tribotroph would not prove that tribotrophy occurs on Europa. It would establish that biology can implement the mechanism somewhere under some set of conditions.

Likewise, measured Earth parameters would not automatically become Europa parameters:

\[
\boxed{
\text{EARTH TRIBOTROPH}
\neq
\text{EUROPA PARAMETER SOURCE BY DEFAULT}
}
\]

Each use would require an explicit applicability review.

### Technical Trace — TC-14

**Primary CCIDs:** CC-FC-CAUSAL-01, CC-FC7-01, CC-NR-01  
**Novelty status:** first-ever claim not earned  
**Positive pilot:** evidence of biology, not tribotrophy  
**Negative pilot:** weak exclusion power  
**New `[SIM]`:** none

---

## TC-15 — What We Need to Know Next

By the end of the project, the unresolved list was too large for a generic “future work” section to be useful. Some unknowns can stop the architecture entirely. Others matter only if a particular metabolic branch becomes active. Some are prerequisites to simulation, while others would improve detail without changing the current project state.

The Needed Areas of Research phase therefore organized future work by **decision leverage**.

The controlling principle is:

> **Research should be ordered by what can change the project state next, not by what is most interesting to calculate.**

### Priority 1 — EF-1

The highest-priority experiment remains the K1 useful-transfer test.

The representative hydrated sealed system must demonstrate that it can:

1. separate charge;
2. export useful charge through a controlled load;
3. couple the transfer into the intended redox or routing chemistry;
4. close countercharge;
5. reset;
6. repeat the cycle.

A low but nonzero useful-transfer result would change downstream sizing. A mechanism-family failure would stop the current architecture and force redesign.

### Priority 2 — EF-MS1

Once EF-1 justifies larger-array work, electrical source behavior and mechanical burden must be measured in the **same array** across current, force, moment, spacing, density, geometry, flow, and dynamic state.

This is the empirical prerequisite for a serious K1-versus-anchor maximum-size crossing.

### Priority 3 — biological K1 support

The project then needs to know how much functional K1 structure a biological support system can construct, coordinate, nourish, anchor, maintain, and replace.

Source area is not free. Generator tissue must be biologically supported.

### Priority 4 — determine whether prey is actually competitive

Before invoking producer branches as maximum-size rescues, Fulgoray must be tested to determine whether prey supply is truly competitive with K/A/R as the first major ceiling.

If K1 support, anchoring, or repair fail much earlier than prey, replacing prey with a producer system may not increase maximum size at all.

### Priority 5 — durability and replacement

The repair problem requires empirical bounds on:

- service life;
- failure mode;
- failure locality;
- replacement rate;
- downtime;
- correlated failure;
- fouling or deposition where decision-bearing.

The relevant quantity is not simply “how long does the material last?” but whether the organism can sustainably replace what fails.

### Priority 6 — sustainable prey, if prey remains active

If prey remains competitive after earlier constraints are better bounded, the ecology must move beyond static density analogues toward real feeding supply:

- prey flux;
- replenishment;
- depletion;
- capture;
- retention;
- ingestion;
- assimilation;
- interference between feeding and K1 hydrodynamics.

Only then does prey become suitable for a decision-bearing integrated maximum model.

### Priority 7 — bind the Fulgoray maximum

A serious integrated Fulgoray maximum solver becomes worthwhile only after K/A/R and prey are bounded strongly enough that the output would not simply reflect invented parameters.

### Priorities 8–14 — activate later branches only when warranted

Fulgorad becomes decision-relevant only if prey is shown to be an important Fulgoray ceiling. Its required matched subsidy trajectory is:

\[
s\mapsto
\{r_P,\kappa_I,I_{\rm subsidy},V_{DH},j_{DH}\}
\]

Fulgorad and Fulgoral then require an empirical loaded direct-host relation:

\[
j_{DH}(V)
\]

Fulgoral additionally requires a defensible producer burden \(\Gamma_{\rm prod}\), followed by persistent material closure \(Z\) for externally required carbon, nitrogen, phosphorus, sulfur, trace metals, ions, and other unrecycled matter.

Only after legitimate host-only direct-interface modularity (**DH-MOD**) is exhausted should Fulgoraz be invoked as a unique rescue. Fulgoraz then requires a frozen internal-symbiosis modularity (**IS-MOD**) topology and empirical bounds on \(j_{HS}\), network capacity/resistance/geometry/durability, and symbiont-to-host metabolite transfer.

### Frozen decision order

The retained ordering is:

> **EF-1 → EF-MS1 → K1 support → Fulgoray prey checkpoint**  
> **→ durability/replacement → prey if active → bound Fulgoray**

and, when later branches are actually activated:

\[
\text{Fulgorad}
\rightarrow
j_{DH}(V)
\rightarrow
\Gamma_{\rm prod}
\rightarrow
Z
\rightarrow
DH\text{-MOD}
\rightarrow
IS\text{-MOD}
\rightarrow
j_{HS}/Network/Transfer
\]

This is a **decision order**, not a prohibition against preparing multiple experiments in parallel. It specifies which results can legitimately change the scientific state of the project next.

### Five future models remain deliberately unrun

All five retained future simulations remain:

> **S0 — NOT ADMITTED / NO RUN**

#### SIM-FUT-01 — shared K1/anchoring crossing

Requires EF-MS1 same-array electrical and mechanical measurements plus biological support bounds.

#### SIM-FUT-02 — integrated Fulgoray corridor

Requires sufficiently bounded K/A/R and sustainable prey if prey remains competitive.

#### SIM-FUT-03 — branch extension comparison

Requires a bounded Fulgoray baseline and branch-specific empirical relations for Fulgorad and Fulgoral.

#### SIM-FUT-04 — Fulgoraz network solver

Requires a demonstrated terminal Fulgoral direct-host limitation, failed DH-MOD rescue, frozen IS-MOD topology, and bounded host-symbiont/network/transfer relations.

#### SIM-FUT-05 — Europa transport/detectability

Requires defensible organism source rates, population distribution, environmental fate, transport, accessible reservoirs, and instrument geometry.

### No-run can be a completed scientific result

These missing simulations are not unfinished computation. Running them now would require the project to assign numerical values or distributions to variables already identified as decision-bearing empirical unknowns.

That would create precision without increasing authority.

The correct next step is therefore experimental rather than computational.

### Scoped backtracking

Future evidence does not automatically invalidate the entire project. A new result should first receive an evidence disposition and then trigger only the necessary project action:

- **NO ACTION**
- **CLAIM-LEVEL SUPERSESSION**
- **SENSITIVITY CHECK**
- **SCOPED BACKTRACK**
- **OWNER-CONTROLLED REDESIGN**

The governing rule is to identify the first affected dependency and rerun only the chain that genuinely depends on it.

A low EF-1 efficiency, for example, may require new sizing without invalidating every environmental or biological result. A complete mechanism-family EF-1 failure is much more serious because the source architecture itself would have to change.

### Technical Trace — TC-15

**Primary CCIDs:** CC-NR-01, CC-FUTSIM-01  
**Highest-priority empirical frontier:** EF-1  
**Global stop condition:** family-level EF-1 failure  
**Future models:** SIM-FUT-01 through SIM-FUT-05 all remain S0  
**New NR empirical achievements:** none

---
# Part V — Methods, History, and What Survives

## TC-16 — Methods, Computation, and Reproducibility

The earlier Parts describe the hypothetical biology and the constraints placed on it. This Part explains how the project decided which quantitative results were allowed to carry scientific authority.

The Europa execution used literature synthesis, analytical calculations, symbolic equations, local Python runs, large parameter grids, and qualitative biological reasoning. Those activities were useful for different purposes, but the project deliberately did **not** treat them as interchangeable forms of evidence.

The central computational rule is:

> **A quantitative claim may be called `[SIM]` only when it is tied to an admitted model, an executable retained artifact, an identifiable run state, retained inputs and outputs, appropriate QA, and enough environment/provenance information for an independent person or future session to reconstruct what was actually executed.**

The scientific principle is not that one particular computer must be used. It is that the boundary between calculation, execution, retained evidence, and interpretation must remain reconstructable.

### What does not automatically count as `[SIM]`

The following may be useful technical work without qualifying as an executed simulation result:

- an equation;
- symbolic algebra;
- a unit conversion;
- a hand calculation;
- an analytical threshold;
- an LLM-generated calculation;
- a proposed parameter sweep;
- unexecuted code;
- preview output from an unauthorized environment;
- a literature value;
- an unretained spreadsheet result;
- output without identifiable producing code or configuration.

The distinction matters because a polished equation or precise numerical answer can look like a computational result even when no controlled run produced it. Such work should be labeled according to what it actually is rather than promoted to `[SIM]`.

### Simulation admission comes before execution

The mature workflow begins by asking:

> **Would this run answer a decision-bearing question using sufficiently defensible inputs and topology?**

If the answer is no, the correct status is:

\[
\boxed{S0=\text{NOT ADMITTED}}
\]

and the correct action is:

\[
\boxed{\text{NO RUN}}
\]

This rule blocked the five major future models described in TC-15. The project already knew that their outputs would be dominated by unresolved empirical assumptions, so running them would have added numerical detail without adding scientific authority.

### Freeze the model before executing it

Once a model is admitted, the project freezes the relevant computational state before execution:

- topology;
- system boundary;
- equations;
- parameter definitions;
- units;
- input ranges;
- exclusions;
- acceptance and failure criteria;
- QA checks;
- expected artifacts.

Only then is the run executed.

Completion by itself does not make a simulation canonical. The mature sequence is:

1. execution;
2. raw-artifact retention;
3. QA;
4. frame, scale, and topology audit;
5. interpretation;
6. owner or project approval where required;
7. promotion to current `[SIM]`.

This prevents a technically successful computation from acquiring authority before anyone has checked whether the model answered the intended question.

### Execution location is not scientific authority

Many canonical Europa runs were executed locally by the project owner on an Apple-silicon workstation. That was a custody and authorization choice, not a claim that the hardware platform is scientifically privileged.

The reusable rule is:

\[
\text{CONVENIENT EXECUTION LOCATION}
\neq
\text{SCIENTIFIC AUTHORITY}
\]

A controlled workstation, HPC system, cloud environment, CI pipeline, or container can support the same method if the execution state and provenance are adequately preserved.

### P0-A as a provenance example

The P0-A execution retains exact script identity, SHA-256, timestamp, output bundle, Python version, platform, package versions, and programmed QA.

| Field | P0-A execution |
|---|---|
| UTC timestamp | `2026-08-27T16:10:53.327945+00:00` |
| Python | `3.13.15` |
| Platform | `macOS-26.5.1-arm64-arm-64bit-Mach-O` |
| NumPy | `2.5.2` |
| pandas | `3.0.5` |
| SciPy | `1.18.0` |
| Script SHA-256 | `f33a44ea6b1a3aa77a9e176670f2e010b85307fe804c98fee41a18f2521885e1` |

That record identifies what actually ran. It does not mean an independent reproduction must use the same machine or package stack if the model is otherwise reproduced correctly.

### Numerical richness does not broaden scientific authority

SIM-EU-06 generated large grid tables and passed 17/17 QA checks. Its authority nevertheless remains narrowly defined:

> **array burden versus required useful-charge fraction**

It does not establish actual interface efficiency, loaded K1 voltage, final geometry, or final organism size.

\[
\boxed{
\text{MORE ROWS}
\neq
\text{BROADER SCIENTIFIC AUTHORITY}
}
\]

A large simulation can explore one narrow question extremely thoroughly while remaining silent about neighboring unknowns.

The same rule applies to T8-O / SIM-EU-24. That computation contained 2,192,832 decision rows and passed 15/15 QA, yet later topology changes made the result nonportable to the final producer branches:

\[
\boxed{
\text{VALID EXECUTION}
\neq
\text{PORTABLE EXECUTION}
}
\]

The computation remains real and valid in the topology that produced it. It simply cannot be transferred into a different circuit architecture without rederivation.

### Input provenance matters as much as code provenance

A preserved script is scientifically weak if nobody can reconstruct why its inputs were chosen.

Decision-bearing inputs should retain, where relevant:

- value or range;
- units;
- evidence status;
- applicability;
- source;
- environmental or experimental conditions;
- transformation or preprocessing;
- topology;
- uncertainty;
- decision role.

A script that can be rerun perfectly with unexplained inputs does not reproduce the scientific reasoning that produced the result.

### Hashes identify artifacts; they do not validate them

SHA-256 is useful because it establishes whether two artifacts are byte-identical. It does not establish that their equations, assumptions, biological interpretation, or scope are correct.

\[
\boxed{
\text{HASH MATCH}
\neq
\text{SCIENTIFIC VALIDATION}
}
\]

Likewise:

\[
\boxed{
\text{GIT}
\neq
\text{REPRODUCIBILITY BY ITSELF}
}
\]

Version control is valuable, especially for the project's GitHub publication and archival workflow, but a repository does not replace model definition, run provenance, input documentation, QA, and interpretation.

### Minimum provenance bundle

For a load-bearing `[SIM]`, the mature method expects at least:

1. exact executable artifact;
2. input state;
3. model identity and topology;
4. run identity;
5. relevant execution environment;
6. raw output;
7. QA;
8. interpretation scope.

Strong additional records include hashes, commit identity, random seed where relevant, container digest, exact command, runtime, warnings, machine-readable outputs, and a README or run note.

### Reproduction levels

The project distinguishes several levels of reproducibility:

- **R0 — Narrative only**
- **R1 — Code recoverable**
- **R2 — Run reconstructable**
- **R3 — Run auditable**
- **R4 — Independently reproduced**

These levels describe provenance and reproducibility, not scientific correctness. A wrong model can be reproduced perfectly.

### Current run classes

The principal minimum-creature chain, SIM-EU-01 through SIM-EU-17, contains many strongly normalized runs, with historical or superseded exceptions such as SIM-EU-07 and SIM-EU-15.

Gate-G runs SIM-EU-18 through SIM-EU-23 retain output-level authority, although exact script and run-package normalization remains incomplete for several subruns. SIM-EU-24/T8-O remains valid historical/nonportable work. NC-EU-01 and NC-EU-02 remain noncanonical execution history.

SIM-FUT-01 through SIM-FUT-05 are different: they were never executed and should never be described as runs.

### Numerical precision is not epistemic precision

A solver may output:

\[
1.824809932
\]

That number can be exactly what the implemented model returned while the underlying biology remains far less certain. Exact machine output should be preserved when needed for reproducibility, but prose should not imply that empirical knowledge has the same precision.

The same principle applies to parameter sweeps. The fraction of a parameter grid that passes a criterion is not a probability unless a probability distribution has actually been defined:

\[
\boxed{
\text{GRID OCCUPANCY}
\neq
\text{PROBABILITY}
}
\]

A grid tells us how modeled states behave across sampled parameter combinations. It does not tell us how likely those states are in nature.

Finally, historical provenance repair must remain separate from scientific repair. Missing hashes, incomplete manifests, or access gaps can sometimes be repaired after the fact. Scientific outputs cannot be invented to fill those documentary holes.

### Technical Trace — TC-16

**Role:** method and reproducibility; no new scientific CCID  
**Method authority:** AP-METH plus METH6-A amendment  
**Permanent controls:** reproducibility \(\neq\) validation; hash \(\neq\) scientific truth; equation \(\neq\) `[SIM]`; a justified no-run can be a completed result

---

## TC-17 — How the Creature Changed

The current Fulgorax architecture can look much more deliberate when described only in final form than it actually was during development. The project did not begin with the final organism and then merely fill in calculations.

It inherited ideas, discovered scope problems, repaired arithmetic, rejected old geometry, opened new metabolic branches, found topology changes, declined simulations that could not yet be justified, and repeatedly narrowed claims that had become stronger than the evidence allowed.

Preserving that history matters because it shows which conclusions were stable, which were repaired, and which survived only within their original scope.

The controlling historical rule is:

\[
\boxed{
\text{PRESERVE THE SCIENCE; UPDATE THE SCOPE}
}
\]

### The pre-Europa concept and the Europa redesign

The current canonical record notes that Fulgorax originated in an earlier speculative atmospheric design that introduced the sealed triboelectric appendage concept and several material ideas. Europa was not treated as a simple location change.

The Europa descendant became attached rather than freely drifting, submerged rather than airborne, exposed to high pressure, dependent on local seafloor flow, concerned with seawater sealing and fouling, electrically coupled to oxygen production, and—within baseline Fulgoray—ecologically dependent on prey.

The relevant historical point for this companion is that the architecture was substantially redesigned for Europa rather than merely transferred into another environment.

### The scale error that became VOID

A prior Europa attempt propagated an incorrect physical scale into downstream calculations. The execution project did not try to rescue those numerical results by applying a simple scaling correction.

It quarantined the numerical branch:

\[
\boxed{
\text{VOID NUMERICS ARE NEVER REUSED}
}
\]

Conceptual questions from a VOID branch may be asked again, but numerical answers must be rederived from the corrected foundation.

This distinction prevents a known numerical error from remaining embedded in later work merely because recalculating from scratch is inconvenient.

### Representative geometry became false canon

Early reconstruction repeatedly used values such as:

- 1.5-mm tribowhips;
- roughly 1,600 tribowhips;
- roughly 0.5–1.0-mm body core;
- roughly 5-mm whole-organism envelope.

Later provenance review showed that repetition had made these numbers appear more authoritative than their derivation justified. The 1.5-mm value is now historical/reference geometry rather than a demonstrated minimum or optimum, while the old whip count, body core, and overall envelope are not current final anatomy.

This became one of the project's central methodological lessons: a convenient modeling point can become false biological canon if downstream work repeatedly treats it as fixed.

### Separated charge stopped being useful electricity

Early versions of the architecture could too easily move from “charge is generated” to “biology has power.”

IC-1 and EF-1 broke that shortcut:

\[
Q_{\rm separated}\neq Q_{\rm usable}
\]

\[
I_{\rm separated}\neq I_{\rm usable}
\]

That change allowed P0-B to remain scientifically useful as a source-side result without pretending it had solved the whole electrical system. P0-C could then ask what useful-transfer fraction would be **required** rather than assigning an efficiency that had never been measured.

### Electrochemistry lost a misleading scalar-energy story

An earlier Gate-A treatment compared food energy and electrolysis cost in a common scalar ledger. Historical values such as `960 kJ/mol O2` and the associated +486/+312 margins entered project reasoning under that framing.

Later audit found that the comparison mixed distinct resource ledgers and included an incorrect oxygen-normalized reference. The mature architecture therefore separated electrical service, prey/metabolic resources, and construction/repair resources.

Those old scalar values remain project history rather than current scientific authority.

### Minimum became a whole-organism question

C1, Gate G, Gate F, Gate H, and C-final progressively forced the subsystem analyses into one coherent reference family.

As a result, “minimum” stopped meaning the smallest favorable geometric row and became:

> **the lowest-complexity lineage-capable whole-organism family not excluded by the complete carried constraints**

That is why the current minimum result is **C8-U / H5-U**, not a body length.

### Food became a gate instead of an assumption

Environmental microbial prey initially entered the concept as an intuitive food source. Gate G forced a more careful distinction between prey concentration and sustainable prey supply and examined the conditions under which throughput could close.

That analysis also opened hydrogen-assisted production, paid electrical farming, and mechanotrophic ecological possibilities. Paid farming was appropriately parked during C-final minimum closure and reopened later when maximum-size scaling posed a different question.

The science did not reverse. The scope of the food question changed.

### Heterotrophy stopped being universal

The minimum-creature campaign was centered on Fulgoray. Maximum-size work later reopened the question of what else K1 electricity might do, producing the four final architectures:

- Fulgoray;
- Fulgorad;
- Fulgoral;
- Fulgoraz.

This expanded the project-wide design space without making the C-final Fulgoray minimum stale. Branch Closure classified the change as a claim-level scope amendment rather than scientific backtracking.

### T8-O survived only inside its own topology

The additive M3-O(+H\(_2\)) architecture received a large real `[SIM]`. Later circuit analysis showed that the final producer branches could not inherit its additive-current accounting.

The correct historical treatment is:

\[
\text{LEGACY}\neq\text{INVALID}
\]

\[
\text{LEGACY}\neq\text{CURRENT CO-EQUAL BRANCH}
\]

\[
\text{OLD `[SIM]` AUTHORITY ENDS AT THE TOPOLOGY BOUNDARY}
\]

The result remains valid history for the model that produced it. It is not a numerical input to the final branch architectures.

### Fulgoraz became harder as it became clearer

Internal symbiosis initially looked like a powerful route around some direct-host producer limitations. Adversarial analysis made the architecture more demanding by exposing its serial dependencies:

- host-to-symbiont electrical service;
- biological network;
- producer cells;
- metabolite transfer;
- oxygen and resource control.

Distributed symbionts do not create additional K1 current, and a local limitation in a direct-host interface does not automatically prove that symbiosis is required. The architecture became less convenient as an abstract rescue and more useful as a testable systems problem.

### Maximum-size work stopped forcing a number

MS9 explicitly asked whether the project had enough empirical authority to admit a decision-bearing maximum-size solver.

It did not.

Instead of assigning distributions to unresolved coefficients, the project stopped. MS11 then retained the joint-admissibility framework, cross-branch structure, shared candidate constraints, and future empirical triggers without manufacturing a maximum size.

### Detection and future research became more constrained

Forward chemistry reduced most apparently distinctive chemical signals to contextual chemistry with substantial confounding. As a result, the strongest detection strategy moved toward a causal mechanism test rather than a search for one unique molecule.

The Needed Areas of Research phase then converted the remaining unknowns into a dependency-ordered program headed by EF-1. The final organizing question became:

> **Which measurement changes the decision next?**

rather than:

> **What can we model next?**

### Technical Trace — TC-17

**Primary CCIDs:** CC-HIST-01, CC-VOID-01, historical CC-T8O-01  
**Historical parent:** retained in current canon only within its original scope  
**VOID rule:** no numerical reuse  
**Policy:** no silent rewriting of historical artifacts

---

## TC-18 — What Survives the Analysis

In this chapter, **survives** has a narrow technical meaning. An idea or architecture survives when it remains **not excluded by the completed desk-science analysis**.

It does not mean demonstrated, observed, validated, probable, or known to exist.

The project began with the proposition that an organism might harvest environmental motion through repeated contact electrification and turn the resulting electrical service into biology. Europa supplied a demanding environment in which to push that idea against mechanics, electrochemistry, ecology, scaling, repair, and biological organization.

Several attractive claims did not survive that process. Some numerical answers disappeared, one numerical branch became VOID, and some real simulations became historical or nonportable. The central mechanism class, however, was not reduced to a known internal contradiction.

### Triboic life survives as a testable mechanism class

The completed desk-science work did not exclude the possibility that a living system could use environmentally driven contact electrification to provide biologically significant electrical or electrochemical service.

The defining chain is:

> environmental motion → biological contact/separation → charge generation  
> → useful loaded transfer → biological/electrochemical service

Many individual links have empirical precedent.

The integrated living chain does not.

That gap is precisely what makes the hypothesis experimentally testable.

### K1 survives as a conditional architecture family

K1 remains the project's principal generator family because the combination of source-side mechanics, underwater contact-electrification precedent, candidate biological material classes, and redox chemistry leaves an open design space.

K1 does not survive as a completed organ. Its final geometry, useful transfer, biological construction, service life, and reset remain unresolved.

The strongest current statement is:

> **K1 remains conditionally admissible until useful loaded transfer/reset is measured.**

### The minimum survives as a family, not a number

For Fulgoray, the retained minimum reference is:

> **C8-U / H5-U CONDITIONAL REFERENCE FAMILY**

A chemically homogeneous unicell is insufficient, but multicellularity was not forced. A compartmentalized unicellular-class architecture remains the lowest-complexity organizational class not excluded.

No scalar minimum body size follows from that result.

### Four architectures remain open

The final branch space contains:

- **Fulgoray** — best-closed reference consumer;
- **Fulgorad** — conditional electrically subsidized consumer;
- **Fulgoral** — conditional direct producer;
- **Fulgoraz** — conditional internal symbiotic producer.

All four remain `[SPEC-INTEGRATED]`. None has a demonstrated numerical maximum, and the branch names do not define an evolutionary, sophistication, or size sequence.

### Maximum size survives as a boundary definition

The maximum-size project did not locate a numerical edge. It established what that edge would mean:

> **the point at which no authorized morphology, modular organization, or biological realization closes every mandatory constraint simultaneously**

K/A/R remains the strongest shared candidate backbone, with branch-specific ecological, resource, and interface constraints added on top.

The mandatory negative conclusions remain:

- no numerical maximum;
- no unlimited-size claim;
- no unique first failure;
- no demonstrated larger maximum for a later branch.

Square-cube effects remain part of that problem because drag, bending moment, support burden, transport distance, and material requirements can scale adversely. They are not a universal one-equation answer because morphology and organization can change as the organism scales.

### Compartmentation remains necessary; multicellularity does not

The organism cannot operate as one chemically homogeneous compartment. The current minimum architecture requires spatial separation of incompatible functions.

A compartmentalized unicellular-class organization remains admissible, while syncytial and multicellular states remain available if empirical constraints force escalation. The project therefore does not predict that real triboic organisms would be unicellular; it says only that multicellularity has not yet been required by the completed analysis.

### Triboelectric energy does not eliminate material ecology

Even Fulgoral and Fulgoraz remain dependent on material inputs:

\[
\boxed{
\text{ENERGY AUTONOMY}
\neq
\text{MATTER AUTONOMY}
}
\]

Electrical service can change how external carbon or prey is used. It cannot eliminate elemental stoichiometry, nutrient requirements, material replacement, or imperfect recycling.

### Repair remains a first-class constraint

No empirical K1 service life has been measured.

More importantly, the project learned that lifetime cannot be interpreted in isolation. Failure locality, replacement cost, renewal rate, and correlated damage matter alongside nominal service life. A short-lived local structure might be sustainable if it can be replaced cheaply and continuously, while a rare catastrophic failure at a K1 root or common support could dominate an otherwise durable appendage.

### The strongest direct test is causal, not chemical

Forward chemistry did not identify a triboic-specific molecule. The strongest direct-detection architecture instead requires a causal package containing:

- biological structure;
- motion or contact;
- electrical output under load;
- perturbation response;
- local chemistry;
- appropriate controls.

The distinctive feature of tribotrophy is the energy-acquisition mechanism, not any one generic metabolic product.

### Earth remains the accessible experimental arena

The staged Earth program can ask progressively stronger questions:

1. Can viable biology be recovered from relevant deep material?
2. Does fresh pressure-retained material reveal more than archived material?
3. Are unusual biological structures associated with flow and electrical activity?
4. Can the defining tribotrophic causal mechanism be demonstrated?

A genuine terrestrial tribotroph would greatly strengthen the mechanism evidence. It would not establish Europa occurrence.

### The moving-fluid census survives as a framework, not a Galactic number

The later FMC work broadens the physical context beyond Europa. Substantial moving fluids can occur in atmospheres, surface liquids, subsurface oceans, hydrothermal systems, supercritical environments, molten interiors, and deep convective envelopes across multiple classes of planetary and substellar bodies.

The census did not earn a preferred Milky Way scalar. \(N_{\rm FM}\) remains an evidence-graded physical-opportunity framework with unresolved terms, explicitly separated from habitability, life, intelligence, and detectability. TC-19 provides the full treatment.

### The research roadmap is itself part of the result

The project does not finish with a generic statement that “more research is needed.”

It finishes with a dependency tree. EF-1 comes first, followed by same-array electrical/mechanical characterization, biological support, prey competitiveness, durability and replacement, and only then the later branch-specific producer problems.

The global stop also remains explicit:

> **GLOBAL STOP / OWNER-CONTROLLED REDESIGN**

if the sealed K1 mechanism family cannot repeatedly export useful charge through a load and reset. Increasing branch complexity cannot hide a source-level failure.

### What did not survive

The final project does **not** support:

- an exact millimeter minimum;
- 1.5 mm as a demonstrated minimum or optimum K1 length;
- roughly 1,600 final tribowhips;
- a fixed roughly 0.5–1-mm body;
- a roughly 5-mm final organism;
- separated charge as proof of useful biological power;
- a known K1 interface efficiency;
- an empirical K1 lifetime;
- D2 as a prediction of Europa prey abundance;
- hydrogen as free food;
- electricity as a universal replacement for matter or food;
- Fulgoraz as the largest or “most advanced” branch;
- a numerical maximum;
- K/A/R as a demonstrated unique first failure;
- H\(_2\), O\(_2\), DIC, organics, or current as triboic-specific signatures;
- remote flyby proof of the deep-seafloor mechanism;
- future model proposals as existing `[SIM]` results.

### What the project did accomplish

After those stronger claims are removed, a substantial technical result remains:

- a defined hypothetical energy-acquisition mechanism;
- a conditional Europa environmental scenario;
- a physically explicit K1 architecture family;
- source-side electromechanical models;
- an electrochemical operating requirement;
- biological demand envelopes;
- a gas-handling architecture;
- conditional food closure;
- durability and organization frontiers;
- a whole-creature conditional Fulgoray minimum family;
- a four-form metabolic architecture space;
- a maximum-size joint-admissibility framework;
- forward-chemistry and confounder analysis;
- a causal detection architecture;
- an Earth experimental program;
- a prioritized empirical roadmap;
- a reproducibility and provenance method.

The whole integrated organism and all four final branches remain:

> **`[SPEC-INTEGRATED]`**

Component `[LAB]` and `[SIM]` evidence cannot be added together arithmetically to turn an untested organism into an empirical fact. Integration has to be demonstrated at the integrated level.

### Final scientific answer

The project cannot answer “yes” to the question of whether life can actually be powered this way.

It also did not earn “no.”

The technically defensible answer is:

> **A family of triboic organism architectures remains not excluded by the completed desk-science analysis, including a conditional lineage-capable Fulgoray minimum reference and three later metabolic extension architectures. No exact minimum body size, numerical maximum size, unique first failure, working K1 interface, integrated organism, or triboic-specific remote chemical biosignature has been demonstrated. The architecture remains empirically unresolved, with repeated useful loaded K1 transfer/reset as its most important architecture-existential test.**

That conclusion is deliberately narrower than proving the organism. It is also much stronger than leaving the concept as an unconstrained thought experiment.

### Where the theory now stands

The central question has changed from:

> “Could I invent a creature that uses triboelectricity?”

to:

> **“Can a specific sealed biological contact-separation system repeatedly export useful electrical service under load, and if it can, can a lineage build and maintain enough of that system to close metabolism, ecology, mechanics, and reproduction simultaneously?”**

The first question is speculative design.

The second can be attacked experimentally.

That transition is one of the project's strongest results.

### Technical Trace — TC-18

**Truth layer:** original 31 frozen Europa CCIDs plus the separate FMC census amendment claims  
**Integrated status:** `[SPEC-INTEGRATED]`  
**Minimum:** Fulgoray C8-U/H5-U conditional reference; no scalar minimum  
**Maximum:** no number, no unique first failure, no later branch demonstrated larger  
**Global empirical priority:** EF-1  
**Detection:** causal direct test; no chemistry-only specific signature  
**Future major `[SIM]`:** all S0  
**Physical-opportunity census:** FMC-14; no preferred Galactic scalar; no biological weighting

---

## TC-19 — How Many Bodies Have Moving Fluids?

The Europa organism project asks whether one biological architecture could use moving water as an energy source. That naturally raises a broader physical question: **how common are bodies with substantial moving fluids at all?**

This is not the same question as habitability. A moving fluid can exist in an environment that is far too hot, cold, chemically hostile, high-pressure, nutrient-poor, or otherwise unsuitable for any known biology. For Triboic Life, fluid motion is only the upstream physical opportunity. Whether a living system can exploit that motion depends on later requirements involving materials, chemistry, energy conversion, biological organization, matter supply, repair, reproduction, and evolution.

The Fluid-Motion Census, finalized in FMC-14, was created specifically to keep those questions separate.

### The quantity being counted

The primary census quantity is:

\[
N_{\rm FM}
\]

defined as the number of **physically distinct present-epoch Milky Way bodies that possess at least one qualifying moving-fluid environment**.

The unit of counting is the body, not the fluid environment. A planet with an atmosphere, a surface ocean, and hydrothermal circulation contributes at most one unit to the primary census. A planet with three independently qualifying moons contributes four bodies if the planet and all three moons satisfy the criteria. This prevents worlds with several fluid environments from being counted multiple times simply because their internal or external fluid systems are complex.

A body qualifies only if three physical conditions are satisfied:

\[
F\land M\land P
\]

where:

- \(F\) = a substantial fluid reservoir exists;
- \(M\) = persistent or recurrent macroscopic motion occurs in that reservoir;
- \(P\) = the reservoir and its motion belong to the present-epoch state rather than a trivial or momentary transient.

No universal current speed, shear threshold, Reynolds number, power density, or biological energy threshold is imposed at the census stage. Those quantities depend on the organism or energy-harvesting architecture being considered. FMC asks only whether the physical opportunity for substantial moving fluid exists.

### Fluid environments are broader than oceans

The census uses a nonexclusive environment registry:

- **ATM** — substantial atmosphere or gaseous envelope;
- **SL** — surface liquid;
- **SO** — subsurface ocean or brine;
- **HC** — hydrothermal or internal liquid circulation;
- **SC** — supercritical-fluid region;
- **HF** — high-temperature molten or internal fluid;
- **DEEP** — deep convective fluid envelope.

These categories deliberately extend beyond familiar liquid-water oceans. Primary observations provide examples of the relevant physical classes, including deep atmospheric motion on Jupiter ([Kaspi et al. 2018](https://doi.org/10.1038/nature25793)), planetary-scale atmospheric variability in brown dwarfs ([Apai et al. 2017](https://doi.org/10.1126/science.aam9848)), hydrocarbon lakes on Titan ([Stofan et al. 2007](https://doi.org/10.1038/nature05438)), and a subsurface sea inferred for Enceladus ([Iess et al. 2014](https://doi.org/10.1126/science.1250551)). The biological problems associated with those environments would be radically different.

FMC does not rank these environments by biological suitability. It does not say that water is preferable to a hydrocarbon liquid for hypothetical non-Earth biology, that an ocean is biologically superior to an atmosphere, or that one form of mechanical forcing is easier to exploit than another.

The census is physical first.

### Why the result is an equation rather than one Galactic number

The tempting shortcut is to multiply the number of stars in the Milky Way by some average number of planets, add moons and free-floating planets, and report one very large total.

FMC-14 rejects that approach because the relevant populations do not share one evidence quality, one denominator, or one well-constrained fluid-bearing fraction. Giant planets and brown dwarfs may have very strong physical reasons to contain moving fluids while their exact Galaxy-wide normalizations remain uncertain. Rocky planets are abundant within observed survey domains, but the fraction retaining substantial atmospheres, surface liquids, or subsurface oceans cannot be represented by one universally supported number. Exomoons have strong Solar System precedent but no sufficiently mature occurrence distribution for a simple Milky Way multiplier. Free-floating planets, compact-host systems, dwarf planets, and minor planetary bodies introduce additional demographic and classification problems.

The primary census is therefore represented as:

\[
\boxed{
N_{\rm FM}
=
\sum_h
\int_{\Omega_h}
\Phi_h(\boldsymbol{x})
\,\chi_{\rm body}(\boldsymbol{x})
\,\mathbf{1}
\!\left[
\bigvee_e Q_e(\boldsymbol{x})
\right]
\,d\boldsymbol{x}
}
\]

Here:

- \(h\) is a mutually exclusive host or dynamical class;
- \(\boldsymbol{x}\) is the body-state vector;
- \(\Phi_h(\boldsymbol{x})\) describes the present Galactic population distribution;
- \(\chi_{\rm body}(\boldsymbol{x})\) determines whether the object falls within the admitted planetary or substellar body scale;
- \(Q_e(\boldsymbol{x})\) records whether environment class \(e\) qualifies.

The logical OR over environments ensures that one body with several qualifying fluid systems still enters the primary census only once.

### An incomplete census should remain visibly incomplete

Because some population terms are not numerically resolved, the current census state is represented as:

\[
\mathcal C^{(s,m)}
=
\left(
N_{\rm numeric}^{(s,m)},
\mathcal U^{(s,m)}
\right)
\]

where \(N_{\rm numeric}^{(s,m)}\) is the subtotal from admitted numerical terms and \(\mathcal U^{(s,m)}\) is the set of unresolved terms retained symbolically.

The important methodological point is that an unresolved population is **not zero**. Missing terms remain visible rather than disappearing from the equation simply because they cannot yet be converted into a trustworthy number.

This makes the census less visually satisfying than a single Galactic estimate, but more useful. New survey results or population constraints can be inserted later without pretending that today's unknowns were ever solved.

### Evidence states

FMC distinguishes four numerical/evidentiary states:

- **FMC-E** — empirically credited numerical terms;
- **FMC-C** — evidence-bounded conditional terms;
- **FMC-M** — explicit model-extended branches;
- **FMC-PARK** — physically interesting populations that do not yet have sufficient evidence for numerical admission.

Population abundance and fluid qualification are treated as separate axes. A body class can be well counted while its fluid-bearing fraction remains poorly known. Conversely, fluid motion can be physically secure for an individual class while the Galactic abundance of that class remains uncertain.

Before a population term enters the numerical subtotal, the census requires the relevant denominator, overlap structure, epoch, portability, and counting unit to be resolved. These gates prevent several common errors, including double-counting overlapping populations, mixing formation rates with present-day inventories, applying an occurrence rate outside the survey population that supports it, or adding a planets-per-star rate directly to a body count without converting the denominator correctly.

### A Solar System census is simpler, but still not automatic

The same framework can be applied locally to the Solar System. FMC-14 deliberately does **not** publish a Solar System scalar, however.

The local problem is easier because the major bodies are individually known, but the qualification rules still matter. Hidden oceans, internal melt layers, substantial atmospheres, hydrothermal circulation, and other candidate fluids differ in evidentiary strength from body to body. A Solar System implementation should therefore be performed as a **body-by-body qualification table** rather than by assuming a familiar list and counting it.

Each candidate planet, moon, or admitted dwarf/minor body would be evaluated for:

1. evidence of a substantial fluid reservoir;
2. evidence of persistent or recurrent macroscopic motion;
3. present-epoch persistence.

Qualifying bodies could carry multiple environment tags—ATM, SL, SO, HC, SC, HF, or DEEP—while still contributing at most one unit to the primary unique-body total.

The useful local question is therefore:

> **How many physically distinct Solar System bodies have at least one substantial fluid reservoir with persistent or recurrent macroscopic motion under the adopted evidence standard?**

That number remains open until the qualification rules are applied consistently.

### Host and body classes beyond ordinary planets

The Galactic ontology is intentionally broader than planets orbiting ordinary main-sequence stars. Host and dynamical classes include bodies associated with ordinary stars, brown dwarfs, free-floating populations, white dwarfs, neutron stars, stellar-mass black holes, mixed-host systems, and additional categories if future observations require them.

Body scale includes giant and substellar objects, conventional planets, Neptune/sub-Neptune bodies, rocky and super-Earth bodies, moons, and sufficiently large dwarf or minor planetary bodies.

FMC-14 identifies several classes for which the existence of moving fluid is physically strong even when the total population remains uncertain: H/He giants, clear Neptune-class bodies, brown dwarfs, bona fide giant free-floating planets, and confirmed giant planets around compact or mixed hosts.

Other classes have the reverse problem. Rocky planets, terrestrial rogues, compact-host rocky worlds, moons, and dwarf/minor bodies may have partially constrained abundance or strong individual examples, while the fraction possessing substantial present-day moving fluids remains poorly known.

Important unresolved terms include:

- moon multiplicity;
- rocky-world fluid-bearing fraction;
- low-mass rogue abundance and composition;
- exclusive Milky Way brown-dwarf normalization;
- dwarf/minor-body abundance;
- compact-host planetary occurrence.

These terms remain unresolved, not zero.

### Environment-specific counts are not additive to the unique-body total

The census can also define environment-specific counts:

\[
N_e
=
\sum_h
\int
\Phi_h(\boldsymbol{x})
\,\chi_{\rm body}(\boldsymbol{x})
\,\mathbf{1}[Q_e(\boldsymbol{x})]
\,d\boldsymbol{x}
\]

but the environment classes overlap. A single body can contribute to several \(N_e\) values while contributing only once to \(N_{\rm FM}\).

Therefore:

\[
\sum_e N_e \neq N_{\rm FM}
\]

in general.

The environment-specific counts are useful for asking how common different physical opportunity classes may be. They should not be summed into a total number of unique bodies without correcting for overlap.

### Why \(N_{\rm FM}\) cannot be converted into a life estimate

The permanent biological firewall is:

\[
\boxed{
N_{\rm FM}
\neq
N_{\rm habitable}
\neq
N_{\rm inhabited}
\neq
N_{\rm intelligent}
\neq
N_{\rm detectable\ civilizations}
}
\]

A moving-fluid census says nothing by itself about whether appropriate chemistry exists, whether abiogenesis occurs, whether a lineage survives, whether complex organisms evolve, or whether intelligence and detectable technology ever appear.

FMC also does not assign biological weights to its fluid classes. A later biological model could define an environment-specific suitability function for a particular organism architecture, but that would be a separate layer placed **after** the physical census.

This separation is especially important for Triboic Life. The census shows that environmental mechanical motion is not conceptually restricted to Earth-like oceans or conventional habitable-zone planets. It does not show that triboic life is common, easy to evolve, or even viable anywhere.

### What can safely be said now

The current companion-level conclusion is:

> **Mechanical-energy environments are not limited to Earth-like oceans or conventional habitable-zone planets. Moving fluids can occur in giant-planet atmospheres, brown-dwarf atmospheres and interiors, volatile-rich planets, subsurface oceans, tidally active moons, free-floating worlds, post-main-sequence planetary systems, and smaller differentiated icy bodies. Current astronomical surveys do not yet permit a single robust Milky Way count of all such bodies. The appropriate result is an updateable, evidence-graded census framework rather than a forced estimate of habitable or inhabited worlds.**

The same rule should govern any future Solar System application: evaluate bodies individually, apply the physical criteria consistently, retain uncertain cases as conditional, and do not convert a census of mechanical opportunity into a biological conclusion.

### Technical Trace — TC-19

**Primary CCIDs:** CC-FMC-01, CC-FMC-02, CC-FMC-BIO-01  
**Project authority:** AP-FMC14 — FMC-14 Final Census Synthesis, Equation Freeze & Frontier Handoff (2026-09-24)  
**External context package:** SP-FMC-01 — representative primary anchors for moving-fluid body classes and selected demographic constraints; not a Galactic census scalar  
**Primary quantity:** \(N_{\rm FM}\), unique present-epoch bodies with at least one qualifying moving-fluid environment  
**Qualification:** substantial fluid + macroscopic motion + persistence/recurrence  
**Counting rule:** one body at most once in the primary census  
**Current numerical disposition:** no preferred Milky Way scalar; unresolved terms remain symbolic or branched  
**Solar System disposition:** framework defined; no scalar Solar System count adopted  
**Biological firewall:** \(N_{\rm FM}\neq N_{\rm habitable}\neq N_{\rm inhabited}\neq N_{\rm intelligent}\neq N_{\rm detectable\ civilizations}\)  
**Citation rule:** FMC-14 is the controlling project synthesis artifact; load-bearing astronomical claims should ultimately trace to the primary literature and FMC source packages rather than relying on the project synthesis alone.

---
# Appendices

## APP-A — CCID Master Index

The **Canonical Claim ID (CCID)** system identifies scientific propositions across the project. A CCID is intended to preserve claim identity even when explanatory prose is reorganized or rewritten.

Editing a report may improve wording, context, or readability. It may not silently change the evidence status, branch scope, topology, unresolved frontier, numerical portability, or prohibited stronger interpretation attached to a CCID.

| CCID | Canonical meaning | Current state | Primary home |
|---|---|---|---|
| **CC-ENV-01** | Europa habitat is a conditional evidence-constrained scenario, not a measured inhabited vent | CURRENT / CONDITIONAL | TC-02 |
| **CC-K1-ARCH-01** | K1 is a speculative integrated sealed tribowhip family; final geometry remains unfrozen | CURRENT / CONDITIONAL | TC-03 |
| **CC-EF1-01** | Separated charge/current does not establish useful loaded transfer; reset remains architecture-existential | UNRESOLVED-EMPIRICAL | TC-04 |
| **CC-P0A-01** | P0-A is a modeled O\(_2\)-demand envelope, not measured Fulgoray demand | CURRENT WITHIN SCOPE | TC-06 |
| **CC-P0B-01** | K1 source/mechanics opportunity survived source-side screens; useful power was not established | CURRENT / CONDITIONAL | TC-04 |
| **CC-P0C-01** | P0-C maps required useful-transfer fraction; no interface efficiency was selected | CURRENT / CONDITIONAL | TC-04 |
| **CC-B2-01** | Repaired B2 bounds electrochemical operating requirements; old scalar framing is superseded | CURRENT + HISTORICAL SUPERSESSION | TC-05 |
| **CC-E-01** | Anchoring was not a modeled minimum/reference kill; final holdfast remains unresolved | CURRENT / CONDITIONAL | TC-04 |
| **CC-IC5-01** | Phase staggering can smooth modeled pulses; real buffering and useful transfer remain unresolved | CURRENT / CONDITIONAL | TC-04 |
| **CC-D-01** | Minimum gas topology favors short local O\(_2\) paths; containment/autotoxicity/material closure remain unresolved | CURRENT / CONDITIONAL | TC-06 |
| **CC-G-01** | Minimum food throughput was not excluded at dense Earth-analogue D2; Europa supply remains unknown | CURRENT / CONDITIONAL | TC-07 |
| **CC-F-01** | No universal K1 durability kill was found; no empirical full-stack service life exists | UNRESOLVED-EMPIRICAL | TC-08 |
| **CC-H-01** | Multicellularity was not forced; compartmentalized unicellular-class architecture is the lowest complexity not excluded | UNRESOLVED-EMPIRICAL | TC-08 |
| **CC-CFINAL-01** | One C8-U/H5-U Fulgoray family survives conditionally; no scalar minimum was earned | UNRESOLVED-EMPIRICAL | TC-09 |
| **CC-MAXDEF-01** | Maximum size is a joint-admissibility family boundary | CURRENT ANALYTICAL | TC-10 |
| **CC-M0-01** | Fulgoray scaling requires simultaneous prey/K1/anchor/repair closure | CURRENT / CONDITIONAL | TC-11.1 |
| **CC-DMIX-01** | Fulgorad can reduce prey pressure while adding electrical burden and retaining matter dependence | CURRENT / CONDITIONAL | TC-11.2 |
| **CC-DAU-01** | Fulgoral can remove prey as the primary fuel/carbon ceiling while adding producer/current/resource constraints | CURRENT / CONDITIONAL | TC-11.3 |
| **CC-ISO-01** | Fulgoraz adds host-symbiont interface, network, and transfer constraints; superiority is unproven | CURRENT / CONDITIONAL | TC-11.4 |
| **CC-MS11-01** | No numerical maximum, unlimited-size claim, unique first failure, or demonstrated M3 \(>\) M0 maximum | UNRESOLVED-EMPIRICAL | TC-10 / TC-11 |
| **CC-T8O-01** | T8-O remains valid historical `[SIM]` only within additive M3-O(+H\(_2\)); it is nonportable | HISTORICAL / NONPORTABLE | TC-11 / TC-17 |
| **CC-FC-H2-01** | Fulgoray H\(_2\) is contextual redox chemistry, not a specific biosignature | CURRENT / NON-SIGNATURE | TC-13 |
| **CC-FC-O2-01** | Producer O\(_2\) is conditional/contextual; no achieved flux or specificity was established | CURRENT / CONTEXTUAL | TC-13 |
| **CC-FC-DIC-01** | CO\(_2\)/DIC and O\(_2\)+DIC patterns are contextual and non-specific | CURRENT / NON-SIGNATURE | TC-13 |
| **CC-FC-K1-01** | Structured functional K1-like material is a future direct-access detection candidate | OPEN / FUTURE TEST | TC-13 |
| **CC-FC-CAUSAL-01** | Strongest direct test is biological structure + motion/contact + loaded electricity + chemistry + controls | OPEN / FUTURE TEST | TC-13 / TC-14 |
| **CC-FC7-01** | No chemistry-only triboic-specific biosignature has been earned; current flyby measurements cannot directly test the mechanism | UNRESOLVED-EMPIRICAL | TC-13 |
| **CC-NR-01** | The unresolved research program is part of the result; NR created no new empirical achievement | NR CLOSED | TC-14 / TC-15 |
| **CC-FUTSIM-01** | Five future major models remain S0 / NOT ADMITTED | S0 / NOT ADMITTED | TC-15 / TC-16 |
| **CC-HIST-01** | Old 1.5-mm / ~1,600 / body-envelope values are historical rather than current anatomy | SUPERSEDED / HISTORICAL | TC-17 |
| **CC-VOID-01** | Incorrect-scale Europa numerical branch is prohibited from numerical reuse | VOID | TC-17 |
| **CC-FMC-01** | \(N_{\rm FM}\) counts unique present-epoch bodies with at least one qualifying moving-fluid environment; one body counts at most once | CURRENT PHYSICAL FRAMEWORK | TC-19 |
| **CC-FMC-02** | Current evidence does not support one preferred Milky Way fluid-motion-body total; unresolved terms remain symbolic or branched | CURRENT / NUMERICALLY UNRESOLVED | TC-19 |
| **CC-FMC-BIO-01** | Fluid-motion opportunity is not equivalent to habitability, life, intelligence, or detectable civilization | PERMANENT FIREWALL | TC-19 |

### APP-A synchronization rule

Any future edit touching one of these claims must preserve, or explicitly revise through project control, its:

- CCID identity;
- evidence state;
- branch and topology;
- mandatory qualifiers;
- numerical-transfer status;
- unresolved empirical frontier;
- prohibited stronger interpretation.

A prose edit alone does not authorize a scientific-state change.

---

## APP-B — Primary Source and Citation Register

### Use rule

External science and internal project state use different authority systems.

**Primary scientific literature** should support claims about what nature, experiments, or observations have demonstrated. **Project artifacts** should support claims about what this project modeled, approved, rejected, superseded, or left unresolved.

A project synthesis may organize or explain external evidence, but it should not replace the primary source when the external scientific claim is load-bearing.

### SP-ENV-01 — Europa environmental context

- [Vance et al. (2018)](https://doi.org/10.1002/2017JE005341)
- [Vance et al. (2021)](https://doi.org/10.1029/2020JE006418)
- [Spiers & Schmidt (2023)](https://doi.org/10.1029/2023JE008028)
- [Marion et al. (2005)](https://doi.org/10.1016/j.gca.2004.06.024)
- [Nozaki et al. (2025)](https://doi.org/10.1016/j.pepi.2025.107450)
- [Byrne et al. (2026)](https://doi.org/10.1038/s41467-025-67151-3)

### SP-FLOW-01 — Earth diffuse-flow analogues

- [Mittelstaedt et al. (2012)](https://doi.org/10.1029/2011GC003991)
- [Mittelstaedt et al. (2016)](https://doi.org/10.1002/2015GC006144)

### SP-EF1-01 — Contact electrification, redox, and reset classes

- [Lin et al. (2020)](https://doi.org/10.1038/s41467-019-14278-9)
- [Ranjan et al. (2026)](https://doi.org/10.1002/anie.202510031)
- [Illera-Perozo et al. (2022)](https://doi.org/10.1039/D2RA01232D)
- [Bertaglia et al. (2024)](https://doi.org/10.1002/admt.202400623)
- [Tang & Ng (2017)](https://doi.org/10.1016/j.biortech.2017.07.189)
- [Milton et al. (2015)](https://doi.org/10.1039/C5SC01538C)
- [Zi et al. (2016)](https://doi.org/10.1038/ncomms10987)

**Critical limitation:** no retained primary benchmark demonstrates the complete repeated hydrated K1 useful-transfer/reset chain.

### SP-B1-01 — OER/HER mechanism families

- [Kanan & Nocera (2008)](https://doi.org/10.1126/science.1162018)
- [Lutterman et al. (2009)](https://doi.org/10.1021/ja900023k)
- [Dincă et al. (2010)](https://doi.org/10.1073/pnas.1001859107)
- [Hayashi et al. (2016)](https://doi.org/10.1039/C6CC07092B)
- [Abe et al. (2021)](https://doi.org/10.1021/acscatal.0c05496)
- [Finn et al. (2024)](https://doi.org/10.1002/celc.202400220)
- [Greene & Madgwick (1991)](https://doi.org/10.1128/AEM.57.4.1114-1120.1991)
- [Kato et al. (2018)](https://doi.org/10.1016/j.electacta.2018.01.133)
- [Hambourger et al. (2008)](https://doi.org/10.1021/ja077691k)
- [Flanagan et al. (2016)](https://doi.org/10.1039/C6CC00515B)

### SP-P0A-01 — Microbial respiration / biological demand

- [Seguro et al. (2025)](https://doi.org/10.5194/bg-22-6225-2025)
- [Cermak et al. (2017)](https://doi.org/10.1038/ismej.2016.161)
- [Zhao et al. (2017)](https://doi.org/10.1128/AEM.02807-16)
- [Fegatella & Cavicchioli (2000)](https://doi.org/10.1128/AEM.66.5.2037-2044.2000)
- [Schut et al. (1995)](https://doi.org/10.1099/13500872-141-2-351)
- [Farmer & Jones (1976)](https://doi.org/10.1111/j.1432-1033.1976.tb10639.x)

### SP-P0B-01 — Underwater triboelectricity / flexible mechanics

- [Wang et al. (2021)](https://doi.org/10.1016/j.nanoen.2021.106503)
- [Huang et al. (2025)](https://doi.org/10.1016/j.nanoen.2025.110664)
- [Vivekananthan et al. (2020)](https://doi.org/10.1039/C9NA00790C)
- [Zhang et al. (2020)](https://doi.org/10.1002/adma.202002824)
- [Shelley et al. (2005)](https://doi.org/10.1103/PhysRevLett.94.094302)
- [Virot et al. (2013)](https://doi.org/10.1016/j.jfluidstructs.2013.09.012)
- [Akcabay & Young (2012)](https://doi.org/10.1063/1.4773210)
- [Meng et al. (2023)](https://doi.org/10.1016/j.matt.2023.09.017)
- [Zi et al. (2015)](https://doi.org/10.1038/ncomms9376)
- [Niu et al. (2013)](https://doi.org/10.1039/C3EE42571A)

### SP-H-01 — Biological organization analogues

- [de Almeida et al. (2015)](https://doi.org/10.1128/JB.00186-15)
- [Schulz et al. (1999)](https://doi.org/10.1126/science.284.5413.493)
- [Melis et al. (2000)](https://doi.org/10.1104/pp.122.1.127)
- [Mohr et al. (2013)](https://doi.org/10.1371/journal.pone.0066060)
- [Dayel & King (2014)](https://doi.org/10.1371/journal.pone.0095577)
- [Rannestad (1974)](https://doi.org/10.1083/jcb.63.3.1009)
- [Rosenbaum et al. (1969)](https://doi.org/10.1083/jcb.41.2.600)
- [Vacchiano et al. (1992)](https://doi.org/10.1111/j.1550-7408.1992.tb01288.x)

### SP-MS5-01 / SP-FC-01 — Electrotrophy, conduction, and symbiosis

- [Nevin et al. (2010)](https://doi.org/10.1128/mBio.00103-10)
- [Bose et al. (2014)](https://doi.org/10.1038/ncomms4391)
- [Ranaivoarisoa et al. (2019)](https://doi.org/10.1038/s41467-019-09377-6)
- [Ishii et al. (2015)](https://doi.org/10.3389/fmicb.2015.00994)
- [Tremblay et al. (2019)](https://doi.org/10.3390/catal9020166)
- [Summers et al. (2010)](https://doi.org/10.1126/science.1196526)
- [Pfeffer et al. (2012)](https://doi.org/10.1038/nature11586)
- [Felbeck (1981)](https://doi.org/10.1126/science.213.4505.336)
- [Bright et al. (2000)](https://doi.org/10.1007/s002270050722)

These papers establish relevant **mechanism classes and analogues**, not Fulgoral or Fulgoraz as integrated organisms.

### SP-FMC-01 — Representative moving-fluid / host-class primary anchors

- [Kaspi et al. (2018)](https://doi.org/10.1038/nature25793) — Juno gravity constraints on deep Jovian jet streams; direct example of large-scale atmospheric motion in a gas giant.
- [Apai et al. (2017)](https://doi.org/10.1126/science.aam9848) — planetary-scale atmospheric variability/wave behavior in brown dwarfs.
- [Stofan et al. (2007)](https://doi.org/10.1038/nature05438) — Cassini radar evidence for Titan's hydrocarbon lakes.
- [Iess et al. (2014)](https://doi.org/10.1126/science.1250551) — gravity evidence compatible with a regional subsurface sea on Enceladus.
- [Mróz et al. (2017)](https://doi.org/10.1038/nature23276) — microlensing constraints on unbound or wide-orbit Jupiter-mass planets; useful specifically as a warning against adopting an overlarge rogue-planet normalization.
- [Vanderburg et al. (2020)](https://doi.org/10.1038/s41586-020-2713-y) — giant planet candidate transiting a white dwarf; compact/post-main-sequence host existence example.
- [Wolszczan & Frail (1992)](https://doi.org/10.1038/355145a0) — planet-sized bodies around a millisecond pulsar; compact-host existence example.

These papers support **example physical classes and selected demographic constraints**. They do not, individually or collectively, establish a Milky Way value for \(N_{\rm FM}\). The census equation, evidence gates, overlap controls, and decision not to publish a preferred Galactic scalar remain project-state conclusions of FMC-14.

### Controlled partial packages

**SP-G-01** — mixed citation readiness. Detailed Gate-G claims should rely on controlled project-state conclusions unless the primary source trail has been normalized.

**SP-F-01** — no report-ready primary package establishes assembled K1 lifetime.

**Gate-D organism-specific oxygen-gradient analogues** — used only as generalized capability precedent in TC-06; organism-specific values are not transferred into the Europa model.

### Project artifact packages

- **AP-CTRL** — source discipline, execution controls, roadmap, revisit ledger
- **AP-CFINAL** — C-final and consolidated minimum-creature state
- **AP-MS11** — MS11 and consolidated maximum-size state
- **AP-BC** — branch closure and scope correction
- **AP-FC7** — forward-chemistry terminal result
- **AP-NR** — research/frontier closure
- **AP-FZ** — final claim/citation/`[SIM]`/wording freeze
- **AP-METH** — method and reproducibility controls
- **AP-FMC14** — Fluid-Motion Census final synthesis and equation freeze; a physical-opportunity framework, not primary astronomical evidence

Project shorthand should resolve to stable repository references or repository-relative links in the public release package.

---

## APP-C — `[SIM]` / Run Provenance Register

This register separates a run's **existence**, **current scientific authority**, and **authorized interpretation**. A completed run may be current, historical, superseded, nonportable, or noncanonical depending on later audit and topology changes.

### Main Europa run chain

| Run | Stage | Current authority | QA / retained identity | Authorized use |
|---|---|---|---|---|
| **SIM-EU-01** | P0-A biological O\(_2\) demand | CURRENT | script SHA `f33a44ea...85e1`; environment retained | biological-demand test family; not measured organism demand |
| **SIM-EU-02** | P0-B low-flow mechanics | CURRENT / scoped | script `step04b2a_mechanical_opportunity.py`; SHA `9812d3f9...3852` | low-flow mechanical opportunity |
| **SIM-EU-03** | P0-B cycle/contact envelope | CURRENT / scoped | run archive retained; SHA `f0d93c53...c674` | frequency/contact sensitivity |
| **SIM-EU-04** | P0-B separated charge/current | CURRENT / scoped | SHA `2f0426fa...a48a` | \(Q_{\rm sep}\) / \(I_{\rm sep}\) only |
| **SIM-EU-05** | P0-B conditional source power | CURRENT / scoped | SHA `7555fdc9...0f8f` | all-separated conditional source power |
| **SIM-EU-06** | P0-C useful-fraction frontier | CURRENT | QA 17/17; SHA `462746d2...f0ab` | array burden vs required useful fraction |
| **SIM-EU-07** | Original B2 | HISTORICAL / PARTLY SUPERSEDED | QA 16/16; SHA `8bfefaad...0771` | historical catalyst/core-voltage work only |
| **SIM-EU-08** | Gate E0 array-load bridge | CURRENT / scoped | QA 14/14; SHA `3c51519b...67a2` | conservative force/root-moment bridge |
| **SIM-EU-09** | Gate E1 force/area screen | CURRENT / scoped | QA 10/10; SHA `e60813ac...c080` | mechanical comparator screen |
| **SIM-EU-10** | Gate E2 drag/holdfast moment | CURRENT / scoped | QA 16/16; SHA `1a093593...77e` | nominal holdfast opportunity |
| **SIM-EU-11** | IC-5 temporal conditioning | CURRENT / scoped | QA 15/15; SHA `69b63625...e456` | phase/asynchrony screen |
| **SIM-EU-12** | Gate D O\(_2\)/H\(_2\) transport | CURRENT / scoped | QA 17/17; SHA `104fb8e9...d7f6` | gas-transport consequence screen |
| **SIM-EU-13** | Gate-A repair reference | CURRENT | QA 8/8; SHA `28a56c8f...9dea` | repaired oxygen-energy reference |
| **SIM-EU-14** | Repaired B2 | CURRENT | QA 13/13; SHA `b4118418...1512` | current electrochemical requirement |
| **SIM-EU-15** | Initial repaired C1 | HISTORICAL / SUPERSEDED | QA 22/22; SHA `c64e3034...0edd` | repair chronology |
| **SIM-EU-16** | C1 PATCH-02 | CURRENT | QA 27/27; SHA `9ce8c5fc...1426` | integrated consequence/operating maps |
| **SIM-EU-17** | C1 PATCH-03 | CURRENT | QA 13/13; SHA `17aa9916...5011` | source-power conservation screen |

### Gate-G output-level provenance

| Run | Function | State | Limitation |
|---|---|---|---|
| **SIM-EU-18** | G0 food-demand translation | CURRENT | exact script/run package not fully normalized |
| **SIM-EU-19** | G1 ambient-prey thresholds | CURRENT | D2 is not a Europa prediction |
| **SIM-EU-20** | G1-A2 comparator closure | CURRENT | no final feeding anatomy |
| **SIM-EU-21** | G2 waste-H\(_2\) farm threshold | CURRENT / G2 topology | supplementary route |
| **SIM-EU-22** | G3 paid-farm resizing | HISTORICAL / SCAFFOLDING | nonportable to final branches |
| **SIM-EU-23** | G3 source-power conservation | HISTORICAL / SCAFFOLDING | topology-restricted |

### SIM-EU-24 — T8-O v3

**State:** VALID HISTORICAL / NOT STALE / NONPORTABLE  
**Topology:** additive M3-O(+H\(_2\))  
**QA:** 15/15 PASS  
**Decision rows:** 2,192,832  
**Limitation:** exact T8-O script/archive identifiers remain incomplete for maximal reproduction from the retained report corpus.

The run remains real and valid within its original model. Its numerical authority does not cross into the final producer topologies.

### Noncanonical executions

- **NC-EU-01** — unrepaired Gate-D attempt; provenance chronology only.
- **NC-EU-02** — failed early C1 repair; no scientific authority.

### Future models — explicitly not runs

- **SIM-FUT-01** — shared K1/anchoring crossing — S0 / NOT ADMITTED
- **SIM-FUT-02** — integrated Fulgoray corridor — S0 / NOT ADMITTED
- **SIM-FUT-03** — branch extension comparison — S0 / NOT ADMITTED
- **SIM-FUT-04** — Fulgoraz internal-network solver — S0 / NOT ADMITTED
- **SIM-FUT-05** — Europa transport/detectability — S0 / NOT ADMITTED

These identifiers describe proposed future models. They must not appear in prose as completed simulations.

---

## APP-D — Equation / Model / Parameter Register

This appendix collects the project's principal equations and model relations in one place. Inclusion here does not make an equation empirical. Each entry retains the interpretation and evidence limits assigned in the main text.

### Electrical and electrochemical relations

\[
I_{\rm required}=4F\dot n_{O_2}
\]

Portable stoichiometric relation between oxygen-production rate and ideal electron/current requirement. It does not establish actual useful K1 current.

\[
Q_{\rm separated}\neq Q_{\rm usable}
\]

\[
I_{\rm separated}\neq I_{\rm usable}
\]

Permanent project-wide electrical firewalls.

\[
P_{\rm allsep}(V)=VI_{\rm sep}
\]

Conditional source relation using separated current. It is not established useful biological power.

\[
u_{\rm required}
=
\frac{I_{\rm required}}
{I_{\rm separated,array}}
\]

Required useful-transfer fraction. It is not an achieved interface efficiency.

\[
V_{\rm core,pH7}=1.824809932\ \mathrm{V}
\]

SIM-EU-14 modeled pH-7 core operating requirement before routing sensitivity. It is not a measured biological voltage.

### Gas and chemistry relations

\[
2H_2O\rightarrow O_2+2H_2
\]

Ideal retained water-splitting product stoichiometry.

\[
n_{CO_2}
=
R_{CO_2/O_2}n_{O_2}
\]

Symbolic Fulgoray carbon relation; \(R_{CO_2/O_2}\) remains unresolved.

\[
J_{O_2,\mathrm{OER}}
>
J_{O_2,\mathrm{ORR}}
+
J_{O_2,\mathrm{resp}}
+
J_{O_2,\mathrm{other}}
\]

Threshold required for net producer-oxygen export. No achieved export flux is implied.

### Repair and lifetime

\[
T_{K1,\min}
=
\frac{M_R}
{q_R M_{\rm bio}}
\]

Analytical relationship between replaceable K1 mass, biological production capacity, and required minimum service time. Both \(q_R\) and real failure locality remain unresolved.

### Maximum-size framework

\[
\lambda_{\max}
=
\sup
\left\{
\lambda:
\text{all mandatory constraints jointly admissible}
\right\}
\]

Definition of the joint-admissibility boundary. No numerical maximum has been solved.

### Fulgorad

\[
r_P(s)
=
\frac{\dot M_{\rm prey,Dmix}}
{\dot M_{\rm prey,M0}}
\]

\[
\kappa_I(s)
=
\frac{I_{\rm req,Dmix}}
{I_{\rm req,M0}}
\]

A prey/anchor sub-envelope may improve where:

\[
r_P\kappa_I<1
\]

but this is not sufficient to establish whole-branch maximum-size extension.

### Fulgoral

\[
I_{\rm fix,min}=4F\dot n_C
\]

Ideal stoichiometric carbon-reduction current floor.

\[
I_{\rm producer}
=
\Gamma_{\rm prod}(4F\dot n_C)
\]

\(\Gamma_{\rm prod}\) remains unresolved and may not be filled by importing a universal terrestrial electrotroph value.

The persistent matter relation is:

\[
\dot n_{z,\rm ext}
=
\nu_z
[\dot M_G+(1-r_z)\dot M_T+\dot M_{\rm export}]
\]

with the permanent firewall:

\[
\text{ENERGY AUTONOMY}
\neq
\text{MATTER AUTONOMY}
\]

The branch also contains the dependency:

\[
K\rightarrow R\rightarrow Z\rightarrow I\rightarrow K
\]

as an accounting topology. No loop gain or stable operating point has been established.

### Fulgoraz

The serial conceptual architecture is:

\[
K1
\rightarrow
HS
\rightarrow
Network
\rightarrow
Symbiont
\rightarrow
Transfer
\rightarrow
Host
\]

with total current conservation:

\[
\sum_m I_m=I_{\rm total}
\]

Distributed producer modules do not create additional source current merely by subdivision.

### Fluid-Motion Census

Primary unique-body census:

\[
N_{\rm FM}
=
\sum_h
\int_{\Omega_h}
\Phi_h(\boldsymbol{x})
\,\chi_{\rm body}(\boldsymbol{x})
\,\mathbf{1}
\!\left[
\bigvee_e Q_e(\boldsymbol{x})
\right]
\,d\boldsymbol{x}
\]

Evidence-limited census state:

\[
\mathcal C^{(s,m)}
=
\left(
N_{\rm numeric}^{(s,m)},
\mathcal U^{(s,m)}
\right)
\]

Environment-specific count:

\[
N_e
=
\sum_h
\int
\Phi_h(\boldsymbol{x})
\,\chi_{\rm body}(\boldsymbol{x})
\,\mathbf{1}[Q_e(\boldsymbol{x})]
\,d\boldsymbol{x}
\]

Because environment classes overlap:

\[
\sum_e N_e\neq N_{\rm FM}
\]

The permanent biological firewall is:

\[
N_{\rm FM}
\neq
N_{\rm habitable}
\neq
N_{\rm inhabited}
\neq
N_{\rm intelligent}
\neq
N_{\rm detectable\ civilizations}
\]

**Current status:** the FMC framework is frozen under FMC-14. No preferred Milky Way scalar and no Solar System scalar are adopted in this companion.

### Parameter-status summary

| Parameter | Current status |
|---|---|
| interface efficiency \(\eta_{\rm interface}\) | NOT AUTHORIZED / NOT MEASURED |
| useful K1 loaded V-I relation | UNRESOLVED-EMPIRICAL |
| final K1 geometry | UNFROZEN |
| numerical minimum K1 thickness | NOT ADOPTED |
| K1 service life | UNRESOLVED-EMPIRICAL |
| repair locality | UNRESOLVED-EMPIRICAL |
| specialized material production \(q_R\) | UNRESOLVED-EMPIRICAL |
| D2 ~\(10^5\) cells/mL | EARTH-ANALOGUE TEST REGIME ONLY |
| \(j_{DH}(V)\) | UNRESOLVED-EMPIRICAL |
| \(\Gamma_{\rm prod}\) | UNRESOLVED |
| \(Z\) resource closure | UNRESOLVED |
| \(j_{HS}\) | UNRESOLVED-EMPIRICAL |
| symbiont network capacity/resistance | UNRESOLVED |
| symbiont-to-host transfer | UNRESOLVED |
| 1.5-mm tribowhip | HISTORICAL / REFERENCE ONLY |
| ~1,600 whips | HISTORICAL |
| ~0.5–1-mm body | HISTORICAL |
| ~5-mm organism | HISTORICAL |
| \(N_{\rm FM}\) Milky Way total | NO PREFERRED SCALAR / FRAMEWORK ONLY |
| Solar System fluid-motion-body total | NOT YET ADOPTED / BODY-BY-BODY APPLICATION REQUIRED |
| biological weighting of fluid environments | OUTSIDE FMC / NOT AUTHORIZED |

This table is intentionally a mixture of unresolved physical parameters, historical values, and prohibited numerical shortcuts. Its purpose is to make the current state obvious before any future calculation reuses one of them.

---

## APP-E — Fulgora Nomenclature and Technical Crosswalk

### Root terms

**Fulgora** — naming root derived from the Roman personification of lightning.

**Triboic life** — the broad hypothetical class of living systems that use self-generated triboelectric charge from environmental mechanical motion for biological electrical or electrochemical service.

**Tribotrophy** — the defining energy-acquisition strategy.

**Tribotroph** — the generic scientific term for an organism using tribotrophy.

**Fulgorax** — the project/common name for a hypothetical triboic organism. The final **x** is treated as a wildcard rather than as a taxonomic designation.

### Final Europa forms

| Reader name | Technical code | Mnemonic | Scientific definition |
|---|---|---|---|
| **Fulgoray** | M0-HET | Y = “Yummy” | Ambient-prey consumer; K1 electricity chiefly supplies O\(_2\)-production service |
| **Fulgorad** | M3-Dmix | D = “Diverse” | Electrically subsidized consumer; external matter dependence remains |
| **Fulgoral** | M3-DA-U | L = “Light” | Direct host producer using electrical bioenergetics for inorganic-carbon fixation |
| **Fulgoraz** | M3-IS(O) | Z = “Zoo” | Internal electro-symbiotic producer with host-to-symbiont electrical service and symbiont-to-host product transfer |

The mnemonics are memory aids only. In particular, “Light” does not imply phototrophy.

The names also do **not** encode evolutionary order, increasing sophistication, or maximum-size ranking. They identify alternative metabolic architectures within the Europa design space.

---

## APP-F — Historical / Superseded / Nonportable / VOID Register

This register preserves old project results without allowing them to drift back into current scientific authority. Historical status does not mean a result never existed, while supersession or nonportability does not necessarily mean the original calculation was internally invalid.

| Item | Current disposition | Current use |
|---|---|---|
| 1.5-mm K1 as minimum/optimum | SUPERSEDED / REFERENCE ONLY | history |
| ~1,600 whips | SUPERSEDED | history |
| ~0.5–1-mm body core | SUPERSEDED | history |
| ~5-mm organism envelope | SUPERSEDED | history |
| old 960 kJ/mol O\(_2\) | SUPERSEDED | method/history |
| old +486/+312 margins | SUPERSEDED | explains ledger repair |
| SIM-EU-07 food-derived break-even/headroom | HISTORICAL / PARTLY SUPERSEDED | chronology |
| SIM-EU-15 first repaired C1 | SUPERSEDED BY PATCHES | chronology |
| G3 paid farming at C-final | HISTORICAL / LATER REOPENED FOR DIFFERENT QUESTION | design history |
| SIM-EU-22/23 G3 scaffolding | HISTORICAL / NONPORTABLE | early source sizing |
| T8-O / SIM-EU-24 | VALID HISTORICAL / NONPORTABLE | topology-control example |
| parent/reference runs | ORIGINAL SCOPE ONLY | history/mechanism |
| NC-EU-01 | NONCANONICAL | provenance chronology |
| NC-EU-02 | NO SCIENTIFIC AUTHORITY | method example |
| incorrect-scale Europa branch | VOID | numerical reuse prohibited |

### Permanent historical rules

\[
\text{HISTORICAL}\neq\text{FALSE}
\]

A historical result may remain an accurate description of what the project once calculated or believed.

\[
\text{SUPERSEDED}\neq\text{NEVER RUN}
\]

Supersession means later controlled work replaced the result as current authority.

\[
\text{VALID IN OLD TOPOLOGY}\neq\text{PORTABLE}
\]

A calculation can remain valid within the model that produced it while being unusable in a later architecture.

\[
\text{VOID}\neq\text{REFERENCE VALUE}
\]

VOID numerics are quarantined. They may be discussed as history but may not be reused as numerical inputs.

The purpose of this register is not archival neatness. It prevents a familiar failure mode in long technical projects: an old number survives in prose, loses its status label, and eventually reappears as though it were current science.

---

## APP-G — Empirical Frontier / STOP / Future-Model Register

This appendix collects the experiments and measurements that can most directly change the scientific state of the project.

### EF-1 — useful loaded sealed-K1 transfer and reset

**Question:** Can a representative hydrated sealed K1 system repeatedly export useful charge under load, close countercharge and redox balance, reset, and return to a reproducible state?

**State:** **UNRESOLVED-EMPIRICAL / HIGHEST-LEVEL EXISTENTIAL FRONTIER**

**Family-level adverse result:** **STOP-01 / OWNER-CONTROLLED REDESIGN**

EF-1 remains the highest-priority experiment because every final Europa branch depends on K1 or an equivalent source mechanism actually delivering useful electrical service rather than merely separating charge.

### Frozen decision order

1. **EF-1** — useful loaded K1 transfer/reset
2. **EF-MS1** — same-array K1 source × force/moment
3. K1 biological support / root productivity
4. Fulgoray prey-competitiveness checkpoint
5. K1 durability and replacement
6. feeding / sustainable prey if still active
7. bind Fulgoray maximum
8. RL-22 Fulgorad if prey-limited
9. loaded \(j_{DH}(V)\)
10. \(\Gamma_{\rm prod}\)
11. \(Z\) persistent resource closure
12. DH-MOD if the direct-host producer interface becomes terminal
13. IS-MOD if DH-MOD fails
14. \(j_{HS}\) / network / transfer

This is a decision hierarchy rather than a prohibition on parallel experimental preparation. Later work can be designed in advance, but it should not be allowed to obscure an earlier architecture-level failure.

### Important minimum-creature frontiers

The minimum-creature result still depends on several measurements that were not available during the desk-science execution:

- real redox-buffer capacity, kinetics, and recovery;
- final loaded K1 source behavior under selected routing;
- integrated separator/electrolyzer compatibility;
- biologically supportable K1 per unit of support tissue;
- coexistence of feeding apparatus and K1 hydrodynamics;
- feeding performance under relevant cold/high-pressure conditions.

These do not all have equal decision priority, but they mark important empirical boundaries around the C8-U/H5-U conditional family.

### Maximum-size frontier

**EF-MS1** requires simultaneous measurement of electrical source behavior and force/moment in the same coherent K1 array as spacing, density, geometry, flow, and dynamic state are varied.

Electrical gain and mechanical burden must belong to the same physical configuration. Combining favorable electrical behavior from one array with favorable mechanical behavior from another would recreate the incoherent-state problem that the maximum-size phase was designed to avoid.

### Fulgorad frontier

The RL-22 requirement is a matched subsidy trajectory:

\[
s\mapsto
\{r_P,\kappa_I,I_{\rm subsidy},V_{DH},j_{DH}\}
\]

All quantities must refer to the same biological/electrical state.

### Fulgoral frontiers

Fulgoral remains limited by unresolved direct-host producer relations:

- \(j_{DH}(V)\);
- \(\Gamma_{\rm prod}\);
- \(Z\), persistent external resource closure;
- DH-MOD, the legitimate host-only modularity space.

### Fulgoraz frontiers

Fulgoraz adds a serial set of unresolved requirements:

- IS-MOD topology;
- \(j_{HS}\);
- network resistance, capacity, geometry, and durability;
- symbiont-to-host product transfer.

These terms must be measured or bounded as a coupled architecture rather than treated as independent optimistic inputs.

### Detection and Earth frontiers

The retained experimental program includes:

- discrimination of functional K1-like material from ordinary biological or mineral debris;
- an integrated causal tribotrophy test;
- the archived-core reanimation pilot;
- fresh pressure-retained follow-up where justified.

The Earth program can strengthen or weaken mechanism-level hypotheses, but biological revival by itself is not evidence of tribotrophy.

### Fluid-Motion Census frontiers

The physical-opportunity census has its own independent unresolved program:

- body-by-body Solar System application of FMC criteria;
- improved exomoon occurrence and multiplicity constraints;
- rocky-planet fluid-bearing fractions;
- low-mass free-floating populations and true-unbound fraction;
- exclusive Galaxy-wide brown-dwarf normalization;
- compact-host planet occurrence;
- extrasolar dwarf/minor-body demographics.

These questions refine \(N_{\rm FM}\). They do not modify the Europa organism architecture unless a future biological model explicitly uses the updated census.

### Global stops

**STOP-01:** family-level failure of sealed-K1 useful-transfer/reset → **OWNER-CONTROLLED REDESIGN**

**STOP-02:** a genuine future contradiction reaching a foundational architecture family → scoped or global stop according to dependency analysis.

The distinction matters because not every negative experiment has project-wide reach. A failed branch-specific producer mechanism may kill that branch while leaving Fulgoray intact. A family-level failure of the defining K1 source mechanism is much more fundamental.

### Future-model admission

SIM-FUT-01 through SIM-FUT-05 remain:

> **S0 / NOT ADMITTED / NO RUN**

until their named empirical prerequisites are met.

---

## APP-H — Reproduction and Audit Checklist

This appendix is intended as a practical control sheet for future reproduction, revision, or extension of the project. It should be usable before reopening an old calculation, transferring a number into a new topology, or writing a new report section.

### Scientific-state reconstruction

Before reproducing or extending a calculation:

- identify the current controlling project artifact;
- identify the relevant CCID;
- identify the branch and topology;
- classify the source as current, historical, superseded, nonportable, or VOID;
- identify the unresolved empirical frontier;
- determine whether later work changed the science, changed only the scope, or changed only the wording.

This step comes first because an old calculation can be perfectly reproducible and still no longer be current.

### Evidence reconstruction

For each load-bearing external claim:

- identify the exact proposition;
- locate the primary source;
- record what was actually measured or observed;
- record the material, system, or organism involved;
- record the experimental or environmental conditions;
- classify applicability to the Europa problem;
- separate the project's inference from the primary result.

The purpose is to prevent an analogue from gradually being rewritten as direct evidence.

### `[SIM]` minimum provenance bundle

Retain:

- executable artifact;
- input state;
- model identity;
- topology and system boundary;
- equations or model version;
- run ID and timestamp;
- execution environment;
- raw output;
- QA;
- interpretation scope;
- explicit nonclaims.

Strong additions include hashes, repository commit, seed where relevant, exact execution command, runtime, warnings, machine-readable tables, and a README or run note.

### Reproduction levels

- **R0 — Narrative only**
- **R1 — Code recoverable**
- **R2 — Run reconstructable**
- **R3 — Run auditable**
- **R4 — Independently reproduced**

A higher reproduction level increases confidence that the computation can be reconstructed. It does not by itself validate the model's scientific assumptions.

### Model-admission checklist

Before a future major simulation, ask:

- Is the decision-bearing question clear?
- Can the result change project state?
- Is the topology fixed?
- Are branch identities fixed?
- Are decision-bearing coefficients sufficiently bounded?
- Are parameter combinations physically and biologically coherent?
- Are acceptance/failure criteria specified?
- Are QA tests defined before execution?
- Are expected outputs and provenance artifacts specified?
- Would an empirical threshold answer the question more directly than another simulation?

If those conditions are not met:

> **S0 / NOT ADMITTED / NO RUN**

### Numerical-transfer checklist

Before transferring a number from one part of the project into another, verify:

- same governing quantity?
- same topology?
- same boundary conditions?
- same scale?
- same physical meaning?
- same electrical/resource/matter-ledger role?
- same applicability?
- no upstream supersession?
- no VOID ancestry?

If equivalence is not established, use:

> **VALID IN ORIGINAL TOPOLOGY / NONPORTABLE**

rather than carrying the number forward.

### Report-writing checklist

Before finalizing any future Triboic Life section, verify that:

- project status comes from the current controlling artifact;
- load-bearing `[LAB]` statements trace to primary evidence;
- project synthesis is not substituted for primary external evidence;
- `[SPEC]` remains visibly speculative;
- Earth analogues remain analogues;
- \(Q_{\rm separated}\neq Q_{\rm usable}\);
- \(I_{\rm separated}\neq I_{\rm usable}\);
- no interface efficiency is invented;
- **PREY DENSITY \(\neq\) PREY SUPPLY RATE**;
- D2 is not described as Europa abundance;
- modeled lifetime scenarios are not called empirical lifetime;
- no scalar minimum is invented;
- no numerical maximum is invented;
- no branch ranking is introduced;
- C-final remains Fulgoray / M0 scope;
- EF-1 remains architecture-existential;
- EF-MS1 remains downstream of EF-1;
- Fulgorad uses coherent matched states;
- \(\Gamma_{\rm prod}\), \(Z\), and Fulgoraz network/interface quantities remain unresolved;
- DH-MOD precedes IS-MOD;
- all five future models remain S0 until admitted;
- Earth reanimation is not called tribotrophy;
- no first-ever experimental claim is made without comprehensive verification;
- \(N_{\rm FM}\) is not described as a habitable, inhabited, intelligent, or civilization count;
- a body is not counted more than once merely because it has several fluid environments;
- no preferred Milky Way or Solar System scalar is invented where FMC retains unresolved terms;
- unresolved census populations are not silently assigned zero;
- no biological ranking of atmosphere, ocean, subsurface, supercritical, or molten-fluid environments is introduced without a separate architecture-specific model.

### Whole-report cold-reader test

A technically capable reader should be able to answer the following questions without reconstructing the entire project history:

- What is tribotrophy?
- What is K1?
- What exactly is EF-1?
- What did P0-A, P0-B, and P0-C actually model?
- What does the repaired B2 voltage mean?
- What is the minimum-creature result?
- Why is there no numerical minimum?
- Why is there no numerical maximum?
- What are the four final Europa forms?
- Why is there no branch ranking?
- Why is T8-O nonportable?
- What has Earth biology demonstrated by analogy?
- What has it not demonstrated?
- Why are H\(_2\), O\(_2\), DIC, organics, and electrical activity non-specific?
- What would constitute a causal tribotrophy test?
- What would positive or negative Earth reanimation mean?
- Which experiment comes first?
- What result stops the current architecture?
- Which future simulations were deliberately not run?
- Which historical numbers are prohibited from reuse?
- Which `[SIM]` runs have strong provenance and which have controlled gaps?
- What does \(N_{\rm FM}\) count?
- What does \(N_{\rm FM}\) explicitly **not** count?
- Why does FMC-14 not publish one preferred Milky Way total?
- How would the same framework be applied body by body to the Solar System without inventing a scalar?

If the report cannot answer those questions clearly, the relevant section requires another audit.

---

# Canonical Lock Record — REP-B1 / FMC-14 Science Amendment

**Canonical artifact:** *Triboic Life: The Technical Companion* — REP-B1 Human-Readable Technical Companion  
**Canonical science base lock:** 2026-09-12  
**FMC science amendment:** 2026-09-24  
**HR5 prose revision approval:** 2026-09-26

The original REP-B1 drafting and audit sequence established the Europa organism state. The later FMC-14 amendment added the moving-fluid physical-opportunity framework without rewriting the earlier organism analysis. It introduced no new Fulgorax `[SIM]`, required no scientific backtracking in the Europa architecture, and adopted no Galactic or Solar System census scalar.

Three cold-reader controls remain part of the locked companion:

1. K1 is presented as a set of **functional regions**, not a frozen anatomical layer stack. Exact order, polarity, and geometry remain unresolved.
2. In TC-18, **survives** means *remains not excluded by completed desk-science analysis*. It does not mean empirically validated.
3. The strongest detection concept is a **conditional causal direct test**, not an earned distinctive chemical biosignature.

The paired-report synchronization rule also requires the causal test to include biological structure, motion/contact, electrical response under load, associated local chemistry, and appropriate mineral/dead-material controls.

### FMC-14 amendment controls

The FMC amendment freezes the following report-level rules:

1. \(N_{\rm FM}\) counts unique present-epoch bodies with at least one substantial persistent or recurrent moving-fluid environment.
2. One body counts at most once in the primary census.
3. Environment classes are nonexclusive descriptors rather than separate primary bodies.
4. Unresolved population terms remain symbolic or explicitly model-branched rather than being invented or silently set to zero.
5. No preferred current Milky Way scalar is claimed.
6. No Solar System scalar is adopted until a body-by-body application has been completed.
7. Physical moving-fluid opportunity remains permanently separated from habitability, life, intelligence, and detectable-civilization counts.

FMC-14 is a synthesis/control artifact. Final publication citations for load-bearing astronomical claims should point to the underlying primary literature used by the FMC phase rather than treating the project synthesis itself as external scientific evidence.

## Final canonical scientific-state statement

> **The Europa Fulgorax project has produced a detailed, internally audited `[SPEC-INTEGRATED]` family of triboic organism architectures that remains not excluded by the completed desk-science analysis. The Fulgoray minimum reference remains C8-U/H5-U and empirically unresolved; no scalar minimum or numerical maximum has been earned; no later branch has demonstrated a larger maximum; no chemistry-only triboic-specific biosignature has been earned; and the architecture-existential EF-1 useful loaded K1 transfer/reset experiment remains the most important next empirical test. Separately, FMC-14 establishes an updateable physical-opportunity framework for counting bodies with substantial persistent or recurrent moving fluids. It does not establish one preferred Milky Way total, does not yet adopt a Solar System total, and does not convert moving-fluid opportunity into a claim about habitability, life, intelligence, or detectable civilizations.**

---

---

## Authorship and AI-assistance disclosure

**Author:** Daniel Moskal. OpenAI ChatGPT assisted with research synthesis, drafting and editing, citation and adversarial audits, and production QA. The author directed the project and approved the final scientific dispositions and text.

*End of REP-B1 — Human-Readable Triboic Technical Companion.*
