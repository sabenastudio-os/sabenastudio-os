
# SabenaStudio Ecosystem  
### AI-powered Digital Architecture by Alejandra Trinca  

---

## Languages  
- Español (versión principal)  
- English version below  

---

# 📚 Índice  

- Descripción General  
- Estructura del Ecosistema  
- Arquitectura General  
- Módulos del Ecosistema  
- Stack Tecnológico General  
- Privacidad y Alcance  
- Autoría y Contacto  
- Agradecimientos  
- English Version  

---

# 🧭 Descripción General  

**SabenaStudio Ecosystem** es el repositorio maestro público que documenta la arquitectura, relaciones internas y funcionamiento general del ecosistema digital creado por **Alejandra Trinca**, especialista en webs inteligentes con IA integrada.  

Este repositorio sirve como punto de referencia para entender cómo interactúan los distintos módulos del sistema, cómo se comunican entre sí y cuáles tecnologías sostienen el ecosistema.  

No contiene código sensible ni claves privadas.  

---

# 🧩 Estructura del Ecosistema  

```
sabenastudio-ecosystem/
│
├── README.md
│
├── quiz/
│   └── README.md
│
└── bot/
    └── README.md
```

El propósito de esta estructura es mantener cada módulo documentado de forma independiente mientras se conserva una visión integral del ecosistema completo.  

---

# 🏗️ Arquitectura General  

```
┌─────────────────────────────────────────────────────────────┐
│                   SABENASTUDIO — ECOSYSTEM                   │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│             Web (Framer)                                    │
│                  │                                          │
│                  ▼                                          │
│         ┌────────────────┐                                   │
│         │   Bot Ale (IA) │                                   │
│         └───▲────────────┘                                   │
│             │                                                │
│     ┌───────┴────────┐                                      │
│     │  Quiz Module   │                                      │
│     └───────┬────────┘                                      │
│             │                                                │
│   ┌─────────▼──────────┐    ┌────────────────────────────┐   │
│   │      Mailgun       │───►│     Email Delivery System   │   │
│   └─────────┬──────────┘    └────────────────────────────┘   │
│             │                                                │
│   ┌─────────▼──────────┐                                    │
│   │   Google Sheets    │                                    │
│   │   Lead Logging     │                                    │
│   └────────────────────┘                                    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

Esta arquitectura resume cómo fluye la información a través del sistema y cómo cada módulo interactúa con los servicios externos.  

---

# 🚀 Módulos del Ecosistema  

## 1. **Quiz de Conversión**  
Módulo interactivo que evalúa al usuario, asigna un puntaje entre 20–100, registra la información en Google Sheets y envía correos personalizados mediante Mailgun.  

Repositorio: **privado**  
Stack: React, Vite, Flask, Railway, Mailgun, Claude  

---

## 2. **Bot Ale**  
Asistente inteligente integrado con Anthropic Claude.  
Orquesta la lógica conversacional y envía correos transaccionales.  

Repositorio: **privado**  

---

# 🛠️ Stack Tecnológico General  

- **Frontend:** React, Vite, Framer  
- **Backend:** Python, Flask, Railway  
- **IA:** Claude, OpenAI, Gemini  
- **Integraciones:** Mailgun, Google Sheets API  

---

# 🔒 Privacidad y Alcance  

Este repositorio no contiene:  
- código privado  
- claves  
- endpoints sensibles  

Su objetivo es documentar y presentar el ecosistema de Sabena Studio en un formato accesible y profesional.  

---

# 🎨 Autoría y Contacto  

Creado por **Alejandra Trinca**  
Especialista en Webs Inteligentes con IA Integrada.  

🌐 **Web:** https://sabenastudio.com  
📧 **Email:** info@sabenastudio.com  
📸 **Instagram:** https://instagram.com/sabenastudio  
🐙 **GitHub:** https://github.com/sabenastudio-os  

---

# 🙏 Agradecimientos  

Este ecosistema fue diseñado con el apoyo de tecnologías modernas como Framer, Railway, Vercel, Google APIs, React, Flask y Anthropic Claude.  
Gracias a todas las personas y herramientas que permiten construir soluciones digitales inteligentes.  

---

# — English Version —

# SabenaStudio Ecosystem  

The **SabenaStudio Ecosystem** is the public master repository documenting the architecture, structure, and functional relationships inside the digital system created by **Alejandra Trinca**, an independent specialist in AI‑powered smart websites.  

This repository does not include private code.  
Its purpose is to provide a professional, high‑level overview of the system.  

---

## 📁 Structure  

```
sabenastudio-ecosystem/
├── README.md
├── quiz/
└── bot/
```

---

## 🧭 Overview  

The ecosystem consists of two documented modules:  

### **1. Quiz Module**  
A conversion‑focused scoring system built with React + Flask.  
It evaluates users, assigns scores, logs data to Google Sheets, and sends automated emails through Mailgun.  

### **2. Bot Ale**  
A custom AI assistant powered by Anthropic Claude.  
Handles conversational logic and transactional emails.  

Both modules integrate with:  
- **Mailgun** (email delivery)  
- **Google Sheets API** (lead logging)  
- **Framer Website** (user entry point)  

---

## 🛠️ Tech Stack  

**Frontend:** React, Vite, Framer  
**Backend:** Flask, Railway  
**AI:** Anthropic Claude, OpenAI, Gemini  
**Integrations:** Mailgun, Google Sheets API  

---

## 🎨 Author & Contact  

Created by **Alejandra Trinca**  
AI‑powered Web Architecture & Digital Ecosystem Design  

Website: https://sabenastudio.com  
Email: info@sabenastudio.com  
Instagram: https://instagram.com/sabenastudio  
GitHub: https://github.com/sabenastudio-os  

---

## ❤️ Credits  

Built with love, curiosity, and modern technologies such as Framer, React, Flask, Railway, Mailgun, Google APIs, and Anthropic Claude.  
