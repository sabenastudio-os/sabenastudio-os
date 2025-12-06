# 🌐 SabenaStudio Ecosystem  
### *AI-powered Digital Architecture by Alejandra Trinca*

[![Ecosystem](https://img.shields.io/badge/SabenaStudio-Ecosystem-black)](#)  
[![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20Flask%20%7C%20Framer%20%7C%20IA-blue)](#)  
[![AI](https://img.shields.io/badge/AI-Claude%20%7C%20OpenAI%20%7C%20Gemini-purple)](#)  
[![Status](https://img.shields.io/badge/Status-Active-success)](#)

---

## Languages  
- **Español (main)**  
- **English version below**

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

SabenaStudio Ecosystem es el repositorio maestro público que documenta la arquitectura, relaciones internas y estructura general de los módulos del ecosistema digital de Sabena Studio.

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

---

# 🚀 Módulos del Ecosistema

## 1. Quiz de Conversión  
Diagnóstico, puntaje, email automático y registro de leads.  
Repositorio: privado.

## 2. Bot Ale  
Asistente IA con lógica personalizada y envíos transaccionales.  
Repositorio: privado.

---

# 🛠️ Stack Tecnológico General

Frontend: React, Vite, Framer  
Backend: Python, Flask, Railway  
IA: Claude, OpenAI, Gemini  
Integraciones: Mailgun, Google Sheets API  

---

# 🔒 Privacidad y Alcance

Este repositorio no contiene claves, código sensible ni endpoints privados.

---

# 🎨 Autoría y Contacto

Creado por **Alejandra Trinca**  
🌐 Web: https://sabenastudio.com  
📧 Email: info@sabenastudio.com  
📸 Instagram: https://instagram.com/sabenastudio  
🐙 GitHub: https://github.com/sabenastudio-os  

---

# 🙏 Agradecimientos

A todas las tecnologías que hacen posible este ecosistema.

---

# 🇬🇧 English Version (Hybrid)

## SabenaStudio Ecosystem

This repository provides the public, high‑level architecture of the Sabena Studio digital ecosystem. No private code is included.

### Structure
```
sabenastudio-ecosystem/
├── README.md
├── quiz/
└── bot/
```

### Overview  
The ecosystem connects three main modules:

- Quiz Module → Lead scoring, email automation, Sheets logging  
- Bot Ale → AI assistant powered by Anthropic Claude  
- Main Website (Framer) → User entry point  

### Tech Stack  
Frontend: React, Vite, Framer  
Backend: Flask, Railway  
AI: Claude, OpenAI, Gemini  
Integrations: Mailgun, Google Sheets

### Contact  
Web: https://sabenastudio.com  
Email: info@sabenastudio.com  
Instagram: https://instagram.com/sabenastudio  
GitHub: https://github.com/sabenastudio-os  
