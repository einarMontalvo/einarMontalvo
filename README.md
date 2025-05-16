# Real-Time PCB Layout & Simulation Tool

A real-time, browser-based circuit board layout and simulation platform inspired by tools like [Flux.ai](https://www.flux.ai). Built with WebGL, React, and FastAPI, this project allows users to draw multi-layer PCBs, simulate circuit behavior, and get immediate visual feedback — all rendered in a smooth, interactive 3D environment.

## 🔧 Tech Stack

- **Frontend**: React, WebGL, Three.js, TypeScript
- **Backend**: Python, FastAPI, Redis (job queue), PostgreSQL
- **Infrastructure**: Docker, AWS ECS/Fargate, S3, CloudFront
- **Communication**: REST API, WebSockets for live data updates

## 🚀 Features

- 🧠 Real-time rendering of circuit layouts with WebGL (60 FPS even under heavy load)
- ⚡ Interactive simulation of component behavior (resistance, voltage, flow)
- 🗂️ Multi-layer board design with drag-and-drop components
- 🔌 Live socket updates for simulation feedback
- 📊 Job queuing with Redis to manage backend compute load
- 🌐 Fully cloud-hosted and scalable via Docker and AWS

## 📈 Performance Wins

- ✅ Reduced backend simulation job timeouts from **30% to under 2%**
- ✅ Increased frontend rendering speed from **~18 FPS to stable 60 FPS**
- ✅ Backend API response times improved by **55%**
- ✅ Supports up to **1,000+ components per board** with minimal lag

## 📷 Demo

![Screenshot](./demo/screenshot.png)

> Example: Simulating power flow across a 4-layer board with live voltage propagation.

## 🛠️ Installation

```bash
# Backend
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload

# Frontend
cd frontend
npm install
npm start
