# VanAdhikar


### Field intelligence for Forest Rights Act implementation


> **Detect the pressure. Explain the signal. Act with confidence.**


VanAdhikar is an interactive monitoring console for exploring synthetic Forest Rights Act (FRA) implementation signals at national, state, and district level. It combines a map-first working surface, explainable rule-based anomaly leads, contextual comparisons, and a bounded AI review assistant that helps a human officer decide where verification should begin.


The project is designed as a transparent prototype for a hackathon setting. It does not make legal determinations, does not expose claimant personally identifiable information, and does not treat an anomaly as proof of wrongdoing.


[Open the live application](https://vanadhikar.onrender.com)


---


## Why VanAdhikar exists


FRA implementation teams often need to move between three different questions:


1. **Where is pressure accumulating?**
2. **Why is a record being surfaced for review?**
3. **What should a human check next?**


VanAdhikar brings those questions into one working surface. The homepage establishes the product story and map context. The console then lets a user move from India-wide signals to a selected state, district, marker, anomaly lead, or comparison row without losing context.


> The prototype boundary is deliberate: district-level records are synthetic and intended for demonstration only. Definitions and reporting vocabulary are anchored to public Ministry of Tribal Affairs and data.gov.in references.[1] [2]


---


## Product experience


| Workspace | What it provides | Why it matters |
|---|---|---|
| **Overview** | National KPIs, implementation pulse, and guided workflow | Establishes the scale and current pressure before investigation |
| **Claims map** | Interactive Leaflet map with claim dots, backlog rings, anomaly emphasis, search, state focus, and district selection | Connects operational signals to geography |
| **Anomalies** | Explainable review leads with risk level, reason, and confidence | Keeps the review path transparent instead of presenting a black-box verdict |
| **State / district comparison** | India-wide state comparison or selected-state district comparison | Lets users identify outliers within the current scope |
| **AI review assistant** | Server-side generated brief containing signal, why it matters, and next human check | Adds AI value while preserving synthetic-data and human-review safeguards |


### A focused interaction model


The console follows a simple operating loop:


```text
Select a scope → locate a signal → inspect the rule → choose the next human check
```


The interface keeps the selected state and district synchronized across the map, search label, comparison scope, selected-district panel, KPIs, review queue, and AI review card.


---


## Highlights


### Map-first investigation


The claims map is built with **Leaflet** and **React Leaflet**. Users can pan, zoom, search for a state or district, toggle map layers, select a marker, and open a marker popup. Selecting a marker updates the Selected District panel and focuses the map on the selected record.
