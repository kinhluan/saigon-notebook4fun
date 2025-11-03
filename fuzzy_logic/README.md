# Fuzzy Logic Traffic Control

Smart traffic lights that think. Fuzzy inference adapts green time based on real-time density.

## What's Inside

- **Full Traffic Cycle**: 🟢 Green → 🟡 Yellow → 🔴 Red
- **4-Direction Input**: North, South, East, West vehicle density (0-100)
- **Fuzzy Controller**: 18 Mamdani rules for intelligent decisions
- **Interactive Demo**: Sliders to test different traffic scenarios
- **Visualizations**: Traffic light animations, membership functions, cycle comparisons
- **Performance Comparison**: Fuzzy vs Fixed-time controller

## Quick Start

Open `Fuzzy_Traffic_Colab.ipynb` in Google Colab. Run all cells. Adjust sliders to simulate traffic.

## The Gist

**Input**: Vehicle density from 4 directions (0-100 cars)

**Fuzzy Variables**:

- Density: Low, Medium, High
- Green time: Short (10-45s), Medium (30-90s), Long (75-120s)

**Example Rules**:

- IF North-South HIGH AND East-West LOW → NS green LONG
- IF East-West HIGH AND North-South LOW → EW green LONG
- IF ALL HIGH → Balanced MEDIUM

**Output**: Optimal green time for each axis (10-120s)

## How It Works

1. **Fuzzification**: 75 cars → "High" (0.8 membership)
2. **Inference**: Apply 18 fuzzy rules (Mamdani)
3. **Defuzzification**: "Long" → 95 seconds green light

Yellow is fixed at 3 seconds. Red time auto-calculated based on opposite axis.

## Test Scenarios

- **🚗 NS Rush**: N=80, S=85, E=15, W=20 → NS gets 103s, EW gets 23s
- **🚙 EW Rush**: N=10, S=15, E=90, W=85 → NS gets 22s, EW gets 104s
- **🚕 Peak All**: N=90, S=85, E=80, W=75 → Balanced 60s each
- **🚐 Off-Peak**: All low → Default 60s each

## Why Fuzzy?

✅ Adapts to real traffic patterns
✅ Reduces wait time (15-30% better than fixed)
✅ Handles asymmetric traffic
✅ No complex math model needed
✅ Works with imprecise sensor data

## Features

- **Interactive Sliders**: Test any density combination
- **Membership Function Plots**: See fuzzy sets visually
- **Cycle Visualizations**: 4-phase traffic light animation
- **Comparison Charts**: Fuzzy vs fixed-time performance
- **Special Cases**: Rush hour, emergency, midnight, balanced

## Real-World Extensions

This could integrate with:

- 📹 AI cameras for density detection
- 🌐 IoT sensors for live data
- 🚑 Priority routing for emergency vehicles
- 📊 ML optimization from historical patterns

---

**Author**: Luân B
