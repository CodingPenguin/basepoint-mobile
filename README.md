# 🧭 Basepoint

**Where do you work, when everywhere’s unfamiliar?**  
Basepoint is the first AI-powered discovery platform for remote workers — helping millions find the perfect café, co-working space, or public workspace anywhere in the world.

---

## 🌍 Why Basepoint?

Remote work is global — but workspaces aren’t.  
Finding a reliable place to work in a new city is slow, frustrating, and inconsistent.

**Google Maps and Yelp weren’t built for remote workers.**  
Basepoint fills that gap with data that actually matters: WiFi speed, noise level, power outlets, crowd vibes, and more.

---

## 🚀 What We’re Building

Basepoint helps digital nomads, creatives, students, and remote professionals:

- 🔍 Discover public workspaces worldwide
- 📶 Filter by WiFi speed, noise, and power access
- 🧠 Get AI-summarized insights based on real reviews
- 📱 Save favorite spots, plan trips, and connect with others

We’re building the **go-to discovery app** for the global remote work generation.

---

## 🛠️ Tech Stack

| Layer        | Stack                          |
|--------------|-------------------------------|
| Mobile App   | Flutter (cross-platform)       |
| Backend      | Firebase (Firestore + Auth)    |
| AI Engine    | LLaMA 3.3:70B via Ollama       |
| Review Parser| Python scripts (CSV → JSON)    |
| Hosting      | Firebase Hosting (upcoming)    |

---

## 🔍 Differentiators

- 📡 **WiFi insights** — not “free WiFi” claims, real speed analysis
- 🔊 **Noise-level summaries** — know the vibe before you show up
- 💰 **Transparent cost data** — minimum spend, coffee prices, coworking rates
- 🧠 **AI summarization** — LLaMA 3.3 condenses dozens of reviews into one clean snapshot
- 🌎 **Global-first** — location data and workspace discovery, city-by-city

---

## 📊 How It Works

1. Scrape Google Maps reviews
2. Clean, group, and enrich data
3. Feed grouped reviews into LLaMA 3.3 via [Ollama](https://ollama.com)
4. Parse key remote-worker data:  
   - WiFi  
   - Cost  
   - Noise  
   - Vibes
5. Output to Firebase for instant mobile access

---

## 🧪 MVP Launch Plan

**Phase 1** (Now):
- Curated launch cities: **Bangkok**, **Manila**, **Tokyo**, **Los Angeles**
- Manual data + AI summaries from Google reviews
- MVP mobile app (Flutter) with search, discovery, and saved spots

**Phase 2** (Beta):
- In-app reviews and uploads
- Real-time updates from community
- Social features and remote collabs

**Phase 3** (Go-To-Market):
- Brand partnerships with cafés and coworking chains
- Paid listing tiers
- Subscription tools for power users

---

## 📂 Repo Structure

```bash
basepoint/
├── input/                  # Raw CSVs (places, reviews)
├── output/                 # Cleaned + AI-enriched JSON
├── scripts/                # Python scripts for data cleaning + enrichment
│   ├── places.py
│   ├── reviews.py
│   └── enrich_places_with_llama.py
├── mobile_app/             # Flutter project folder (WIP)
└── README.md
