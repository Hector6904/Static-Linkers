# Geolocation from Shadows
 
**CTF:** Cipathon '26 — Round 1
**Category:** OSINT
**Difficulty:** Medium
**Solved by:** Hector1516
 
---
 
## Challenge Description
 
> "When I was overseas I visited a nice church, but I can't remember what it was called. To make it worse, the only picture I have is this photo I took nearby. Can you find the name of the nearest church to this location?"
 
**Given image:**
 
![Challenge Image](./1773565855248_image.png)
 
**Flag Format:** `CIPH{CHURCHNAME}`
 
---
 
## Approach
 
### Step 1 — Extract Visual Clues
 
On first look at the image, one detail stood out immediately: the branding **"Oya's"** visible on the building windows. That became the primary search anchor.
 
### Step 2 — Reverse Image Search
 
Tried Google Images first — no useful results. Switched to **Yandex reverse image search**, which returned a location hint pointing to the **Netherlands**.
 
### Step 3 — Narrowing the Location
 
Searched `"Oya's Netherlands"` and identified the full business name as **Oya's Childcare**. Further research revealed there were **3 separate Oya's Childcare locations** across the Netherlands.
 
### Step 4 — Street View Verification
 
Loaded all 3 locations in **Google Maps** and used **Street View** to visually compare each one against the challenge image. One location matched the building's architecture and street layout exactly.
 
### Step 5 — Finding the Church
 
Once the exact location was confirmed, searched the surrounding area on Google Maps for the nearest church — which turned out to be **Obrechtkerk**.
 
---
 
## Flag
 
```
CIPH{obrechtkerk}
```
 
---
 
## Key Takeaway
 
When reverse image search on Google fails, **Yandex** is often more effective for geolocating non-English or European locations. From there, it was a matter of methodically verifying each candidate location via Street View rather than guessing.
 
---
 
## Solve Confirmation
 
![Solve Screenshot](./1773566344043_image.png)
