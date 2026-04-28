# VisionAid 🔵

> **AI-Powered Assistive Glass for the Visually Impaired**

🥇 **Gold Award + Panel's Choice Award — WYSII 2026 (International)**
🏅 Top 5 Project Globally · 🇧🇩 National Bronze Award — WYSII 2026

---

## The Problem

Over 1 million people in Bangladesh live with visual impairment.
Commercial assistive devices — when they exist — cost BDT 80,000–120,000.
Most families cannot afford them. So most people go without.

VisionAid is a prototype that changes that equation.
Same capabilities. ~BDT 9,000–12,000 hardware cost.
Built in Feni, Bangladesh. Tested in the real world.

---

## What VisionAid Does

| Feature | Description |
|---|---|
| 🚧 Obstacle Detection | Real-time path hazard detection with audio alert |
| 👤 Face Recognition | Identifies known people and announces their name |
| 🧳 Object Recognition | Names objects in the environment |
| 🖼️ Scene Description | Describes surroundings in natural language (BLIP) |
| 📖 Book Reading | OCR-based text reading aloud |
| 💵 Currency Detection | Identifies and announces Bangladesh currency notes |
| 🎨 Color Detection | Identifies and announces colors of objects |

All features run **on-device** — no internet required.

---

## Why It Matters

Most AI assistive tech is built for high-income countries.
VisionAid was built *in* Bangladesh, *for* Bangladesh — and beyond.

The hardware is a fraction of the cost.
The model runs on edge hardware without cloud dependency.
The mission is accessibility, not profit.

---

## Technical Architecture

```
Camera Input
     │
     ▼
Preprocessing (OpenCV)
     │
     ├──► Obstacle Detection      [YOLO + OpenVINO]
     ├──► Face Recognition        [Custom model + TFLite]
     ├──► Object Recognition      [YOLO + TFLite]
     ├──► Scene Description       [BLIP]
     ├──► Text/Book Reading       [OCR pipeline]
     ├──► Currency Detection      [Custom classifier]
     └──► Color Detection         [HSV-based detection]
     │
     ▼
Audio Output (Text-to-Speech)
```

**Optimization techniques:** Model quantization · Inference caching · OpenVINO acceleration

---

## Stack

| Layer | Tools |
|---|---|
| Vision Processing | OpenCV |
| Object & Obstacle Detection | YOLOv8 + TensorFlow Lite |
| Scene Understanding | BLIP (image captioning) |
| Edge Inference | OpenVINO, Quantization |
| Audio Feedback | Text-to-Speech pipeline |
| Hardware | Raspberry Pi / edge SBC |

---

## Cost Comparison

| Solution | Estimated Cost |
|---|---|
| Commercial assistive glasses (international) | BDT 80,000–120,000+ |
| **VisionAid prototype** | **~BDT 9,000–12,000** |

**~10× cheaper.** Same core capabilities.

---

## Awards & Recognition

- 🥇 **Gold Award** — WYSII 2026 (International)
- 🏆 **Panel's Choice Award** — WYSII 2026 (International)
- 🌍 **Top 5 Project Globally** — WYSII 2026
- 🥉 **National Bronze Award** — WYSII 2026 (Bangladesh)

---

## Status

**Current:** Working prototype · Award-winning · Under active development
**Next:** Real user testing · Hardware refinement · Expanded language support

---

## About the Builder

Built by **Muhaiminul Abedin Farhan**, 19, from Feni, Bangladesh.
Self-taught AI/ML engineer. Built this during gap year after HSC.

The idea came from watching people lose vision during protests in Bangladesh in 2024.
Not from a business plan. From a real problem, seen with his own eyes.

→ [GitHub Profile](https://github.com/muhaiminul00)
→ [LinkedIn](https://linkedin.com/in/muhaiminul00)

---

## License

This project is open for research and non-commercial use.
If you want to collaborate, improve, or deploy VisionAid — reach out.
