# Social Media Emotion Analysis and Economic Influence

This project explores how social media shapes public opinion and influences economic decisions. It combines real-time tweet analysis with agent-based modeling to simulate emotional impact using **AnyLogic**.

## 📌 Project Overview

Social media plays a powerful role in shaping how people feel and behave. This project uses:
- **Twitter API v2** to fetch real-time tweets
- **Natural language processing** (NLP) to analyze emotions
- **AnyLogic** agent-based simulation to model how social media content affects user emotions over time

It helps researchers and analysts understand how emotions driven by online content might influence consumer decisions, market behavior, or social trends.

## ✨ Features

- ✅ Fetches tweets using Twitter API v2
- ✅ Appends tweet data to a local file (`tweets.txt`)
- ✅ Integrates with an **agent-based simulation model in AnyLogic**
- ✅ Each agent represents a user with unique behavior (memory, attention)
- ✅ Simulates how social media posts affect user emotions using Ekman's model

## 🛠️ Technologies Used

- **Java** – For data collection and file writing
- **OkHttp** – HTTP client to access Twitter API
- **org.json** – For JSON parsing
- **Twitter API v2** – For recent tweet search
- **AnyLogic** – For simulation modeling (`.alp` file)

## 🧠 Agent-Based Modeling (ABM)

The core simulation is implemented in **AnyLogic** using agents that represent users. Each agent:
- Has a memory and attention span
- Reads posts from the collected tweet file
- Updates emotional states based on post content using Ekman’s universal emotions (joy, sadness, fear, anger, surprise, disgust)
- Emotion data is visualized over time in a time-series plot

### Main Simulation File

> The AnyLogic simulation file is:  
> **`social_media_emotion_simulation.alp`**  
> (Open with AnyLogic 8+)

## 📂 Project Structure

```bash
.
├── TwitterSearchToFile.java     # Java code to fetch tweets
├── tweets.txt                       # Appended output file with tweet text
├── social_media_emotion_simulation.alp  # AnyLogic ABM simulation file
├── README.md
└── pom.xml                          # Maven dependencies
