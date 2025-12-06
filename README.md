# 🌐 SabenaStudio Ecosystem  
### *AI-powered Digital Architecture by Alejandra Trinca*

![Ecosystem](https://img.shields.io/badge/Module-Ecosystem-black)
![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20Flask%20%7C%20Framer%20%7C%20IA-blue)
![AI](https://img.shields.io/badge/AI-Claude%20%7C%20OpenAI%20%7C%20Gemini-purple)
![Status](https://img.shields.io/badge/Status-Active-success)

---

## Languages  
- Español (versión principal)  
- [English version](#english-version)  

---

# 📚 Índice  
- [🧭 Descripción General](#-descripción-general)  
- [🧩 Estructura del Ecosistema](#-estructura-del-ecosistema)  
- [🏗️ Arquitectura General](#-arquitectura-general)  
- [🚀 Módulos del Ecosistema](#-módulos-del-ecosistema)  
- [🛠️ Stack Tecnológico General](#-stack-tecnológico-general)  
- [🔒 Privacidad y Alcance](#-privacidad-y-alcance)  
- [🎨 Autoría y Contacto](#-autoría-y-contacto)  
- [🙏 Agradecimientos](#-agradecimientos)  
- [🇬🇧 English Version](#english-version)  

---

# 🧭 Descripción General

**SabenaStudio Ecosystem** es el repositorio maestro público que documenta la arquitectura, relaciones internas y funcionamiento general del ecosistema digital creado por **Alejandra Trinca**, especialista en webs inteligentes con IA integrada.

Su propósito es ofrecer una vista clara, profesional y accesible de cómo operan los módulos principales del sistema.

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

## 1. **Quiz de Conversión**
Módulo que evalúa, puntúa, registra en Google Sheets y envía correos mediante Mailgun.

**Repositorio:** privado  
**Stack:** React, Vite, Flask, Railway, Mailgun, Claude

---

## 2. **Bot Ale**
Asistente conversacional creado sobre Anthropic Claude, con lógica personalizada y envíos transaccionales automáticos.

**Repositorio:** privado  

---

# 🛠️ Stack Tecnológico General

- **Frontend:** React, Vite, Framer  
- **Backend:** Python, Flask, Railway  
- **IA:** Claude, OpenAI, Gemini  
- **Integraciones:** Mailgun, Google Sheets API  

---

# 🔒 Privacidad y Alcance

Este repositorio **no contiene**:  
- claves  
- código privado  
- endpoints sensibles  

Su objetivo es servir como documentación de arquitectura del ecosistema Sabena Studio.

---

# 🎨 Autoría y Contacto

Creado por **Alejandra Trinca**  
Especialista en Webs Inteligentes con IA Integrada.

🌐 Web: https://sabenastudio.com  
📧 Email: info@sabenastudio.com  
📸 Instagram: https://instagram.com/sabenastudio  
🐙 GitHub: https://github.com/sabenastudio-os  

---

# 🙏 Agradecimientos

Gracias a las tecnologías que hicieron posible este ecosistema:  
Framer, React, Flask, Railway, Google APIs, Mailgun, Anthropic Claude y más.  

---

# 🇬🇧 English Version

## SabenaStudio Ecosystem

The **SabenaStudio Ecosystem** is the public master repository documenting the architecture, internal logic and functional connections of Sabena Studio's digital system.

This repository contains **no private code**.  
It serves as a professional, high-level overview for collaborators and clients.

---

## 📁 Structure

```
sabenastudio-ecosystem/
├── README.md
├── quiz/
└── bot/
```

---

## 🧩 Overview

### **Quiz Module**  
Built with React + Flask.  
Evaluates users, assigns a score, logs data in Google Sheets, and sends automated emails through Mailgun.

### **Bot Ale**  
Powered by Anthropic Claude.  
Handles conversational logic and transactional messages.

Both modules integrate with Mailgun & Google Sheets.

---

## 🛠️ Tech Stack

**Frontend:** React, Vite, Framer  
**Backend:** Flask, Railway  
**AI:** Claude, OpenAI, Gemini  
**Integrations:** Mailgun, Google Sheets  

---

## 🎨 Author & Contact

Created by **Alejandra Trinca**  

- Website: https://sabenastudio.com  
- Email: info@sabenastudio.com  
- Instagram: https://instagram.com/sabenastudio  
- GitHub: https://github.com/sabenastudio-os  

---

## ❤️ Credits

Built with curiosity, precision, and modern technologies powering AI-driven digital experiences.
ologies such as Framer, React, Flask, Railway, Mailgun, Google APIs, and Anthropic Claude.  
