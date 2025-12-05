# 🚀 Sabena Studio - Ecosistema Digital Inteligente

[![Status](https://img.shields.io/badge/status-Production-success)](https://sabenastudio.com)
[![AI](https://img.shields.io/badge/AI-Claude%204.5%20Haiku-blueviolet)](https://www.anthropic.com/)
[![Backend](https://img.shields.io/badge/backend-Python%20%7C%20Flask-blue)](#)
[![Frontend](https://img.shields.io/badge/frontend-React%20%7C%20Vite-61dafb)](#)
[![Deploy](https://img.shields.io/badge/deploy-Railway%20%7C%20Vercel-success)](#)

> **Ecosistema de herramientas inteligentes que automatizan la captación, cualificación y conversión de leads para Sabena Studio.**

---

## 📖 Descripción General

**Sabena Studio** by Alejandra Trinca es un estudio digital que combina diseño web estratégico con inteligencia artificial aplicada. Este repositorio público documenta dos proyectos principales que demuestran la implementación práctica de IA conversacional y sistemas de scoring inteligentes para automatizar procesos comerciales.

---

## 🎯 Propósito del Ecosistema

Ambos proyectos fueron diseñados para resolver un desafío clave de los negocios digitales modernos: **convertir visitantes web en leads cualificados sin intervención manual, operando 24/7**.

### Problemas que Resuelve:

- ❌ **Pérdida de leads fuera de horario:** Opera 24/7 sin intervención humana
- ❌ **Tiempo perdido en consultas no cualificadas:** Evalúa automáticamente el nivel de interés
- ❌ **Fricción en el proceso de contacto:** Ofrece diagnóstico inmediato con descuentos o agendado inteligente
- ❌ **Falta de seguimiento estructurado:** Registra cada interacción con datos clave en Google Sheets
- ❌ **Comunicación no profesional:** Emails desde dominio corporativo verificado

---

## 🗂️ Proyectos del Ecosistema

### 1. 🎯 Quiz de Conversión

**Repositorio:** [Quiz-conversion-sabena](https://github.com/sabenastudio-os/Quiz-conversion-sabena) (Privado)

Quiz inteligente que diagnostica necesidades digitales, calcula un score personalizado y envía descuentos automáticamente.

#### Características:
- 📊 **Sistema de scoring inteligente** (20-100 puntos)
- 🎁 **Descuentos personalizados** (15%, 25%, 30%)
- 📧 **Emails automáticos** vía Mailgun desde `contacto@sabenastudio.com`
- 📈 **Registro automático** en Google Sheets
- 🎨 **Interfaz bilingüe** (ES/EN) con diseño responsive

#### Stack Técnico:
- **Frontend:** React + Vite (Vercel)
- **Backend:** Flask + Python (Railway)
- **Email:** Mailgun API
- **Storage:** Google Sheets API

---

### 2. 🤖 Ale Bot - Asistente Virtual con IA

**Repositorios:**
- Backend: [backend-ale-bot](https://github.com/sabenastudio-os/backend-ale-bot) (Privado)
- Frontend: [ale-bot-demo](https://github.com/sabenastudio-os/ale-bot-demo) (Privado)

Asistente virtual estratégico con IA integrada que cualifica leads, registra información y facilita el contacto inmediato.

#### Características:
- 🧠 **IA conversacional** con Claude 4.5 Haiku
- 📊 **Lead scoring automático** durante la conversación
- 📧 **Envío de briefs** vía Mailgun desde `contacto@sabenastudio.com`
- 📱 **Integración con WhatsApp** para seguimiento inmediato
- 📈 **Registro en Google Sheets** con toda la información capturada
- 💬 **Widget embebible** responsive y no invasivo

#### Stack Técnico:
- **Frontend:** React 18 + Vite (Vercel)
- **Backend:** Flask + Python (Railway)
- **IA:** Anthropic Claude 4.5 Haiku API con Function Calling
- **Email:** Mailgun API
- **Integraciones:** Google Sheets API, WhatsApp Business

---

## 🏗️ Arquitectura del Ecosistema

```
┌─────────────────────────────────────────────────────────────┐
│              ECOSISTEMA SABENA STUDIO                       │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌──────────────────┐         ┌──────────────────┐        │
│  │   QUIZ FRONTEND  │         │   BOT FRONTEND   │        │
│  │    (Vercel)      │         │    (Vercel)      │        │
│  │  React + Vite    │         │  React + Vite    │        │
│  └────────┬─────────┘         └────────┬─────────┘        │
│           │                            │                   │
│           │         API REST           │                   │
│           ▼                            ▼                   │
│  ┌──────────────────┐         ┌──────────────────┐        │
│  │  QUIZ BACKEND    │         │   BOT BACKEND    │        │
│  │   (Railway)      │         │   (Railway)      │        │
│  │ Flask + Python   │         │ Flask + Claude   │        │
│  └────────┬─────────┘         └────────┬─────────┘        │
│           │                            │                   │
│           └────────────┬───────────────┘                   │
│                        │                                   │
│           ┌────────────┴───────────────┐                  │
│           │                            │                   │
│    ┌──────▼──────┐            ┌────────▼────────┐        │
│    │   Mailgun   │            │  Google Sheets  │        │
│    │     API     │            │      API        │        │
│    │             │            │                 │        │
│    │  (Emails)   │            │    (Leads)      │        │
│    └─────────────┘            └─────────────────┘        │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## ✨ Características Compartidas

### 📧 Sistema de Email Profesional
- **Remitente corporativo:** `contacto@sabenastudio.com`
- **Infraestructura:** Mailgun API con dominio verificado
- **Templates HTML:** Diseños responsivos y profesionales
- **Deliverability:** SPF + DKIM configurados

### 📊 Gestión de Leads
- **Registro automático** en Google Sheets
- **Captura completa:** nombre, email, empresa, necesidades, presupuesto
- **Análisis de conversión** con datos estructurados
- **Service Accounts** de Google para máxima seguridad

### 🎨 Diseño Profesional
- **UI/UX optimizado** para conversión
- **Responsive design** (mobile-first)
- **Identidad visual** coherente con Sabena Studio
- **Accesibilidad** y usabilidad prioritarias

### 🚀 Infraestructura Escalable
- **Frontend:** Vercel (deploy automático desde GitHub)
- **Backend:** Railway (escalable con 99.9% uptime)
- **Monitoreo:** Logs en tiempo real
- **CI/CD:** Despliegue automático al hacer push

---

## 🛣️ Roadmap del Ecosistema

### ✅ Completado (v1.0 - Producción)
- [x] Quiz de conversión con scoring inteligente
- [x] Ale Bot con IA conversacional
- [x] Integración con Mailgun desde `contacto@sabenastudio.com`
- [x] Registro automático en Google Sheets
- [x] Deploy en Railway + Vercel
- [x] Integración con WhatsApp Business

### 🚧 En Desarrollo (v1.1)
- [ ] Dashboard unificado para revisar leads
- [ ] Analytics de conversión (Google Analytics 4)
- [ ] A/B testing de preguntas y flujos
- [ ] Notificaciones push cuando llega un lead
- [ ] Sistema de seguimiento automatizado

### 🔮 Futuro (v2.0)
- [ ] Integración con CRM (HubSpot / Notion)
- [ ] Lead scoring con Machine Learning
- [ ] Automatización de onboarding de clientes
- [ ] Más idiomas (Portugués, Francés)
- [ ] Integración con redes sociales (LinkedIn, Instagram)

---

## 🔐 Seguridad y Privacidad

- ✅ **Credenciales encriptadas** en variables de entorno
- ✅ **HTTPS obligatorio** en todos los endpoints
- ✅ **CORS configurado** para dominios autorizados únicamente
- ✅ **Service Accounts de Google** con permisos mínimos necesarios
- ✅ **No almacenamiento de datos sensibles** en servidores
- ✅ **Emails desde dominio verificado** (SPF + DKIM)
- ✅ **Google Workspace** para gestión corporativa de emails
- ⚠️ **Cumplimiento GDPR:** En revisión (pendiente para operación en Europa)

---

## 📊 Resultados (Producción)

> **🚀 Proyectos en producción activa**

| Métrica | Quiz | Bot Ale |
|---------|------|---------|
| Tiempo de respuesta | ~1-2s | ~2-3s |
| Disponibilidad | 24/7 | 24/7 |
| Idiomas soportados | ES / EN | ES |
| Costo por interacción | ~$0.02 | ~$0.05-0.10 |
| Email deliverability | 99%+ | 99%+ |

---

## 🎨 Capturas de Pantalla

### Quiz de Conversión
_Interfaz limpia con progreso visual y resultados personalizados_

### Ale Bot
_Widget de chat integrado con conversación natural_

---

## 📄 Licencia

Todos los proyectos del ecosistema Sabena Studio utilizan la Licencia MIT.

**Copyright (c) 2025 Sabena Studio by Alejandra Trinca**

Ver archivos LICENSE en cada repositorio para más detalles.

---

## 👩‍💻 Autora

**Alejandra Trinca**  
Framer Expert Certificada | Desarrollo Web con IA | Automatización Inteligente

- 🌐 Web: [sabenastudio.com](https://sabenastudio.com)
- 📧 Email: [contacto@sabenastudio.com](mailto:contacto@sabenastudio.com)
- 💼 LinkedIn: [linkedin.com/in/alejandra-trinca](https://linkedin.com/in/alejandra-trinca)
- 📱 WhatsApp: [+34 911 807 673](https://wa.me/34911807673)

---

## 🙏 Agradecimientos

- [Anthropic](https://www.anthropic.com/) - Claude AI para asistencia con IA
- [Mailgun](https://www.mailgun.com/) - Infraestructura de email transaccional
- [Railway](https://railway.app/) - Hosting del backend
- [Vercel](https://vercel.com/) - Hosting del frontend
- [Google Cloud](https://cloud.google.com/) - APIs de productividad (Sheets, Workspace)

---

## 💬 Contacto y Soporte

¿Interesado en implementar soluciones similares para tu negocio?

**📱 Contacta por WhatsApp:**  
[Enviar mensaje](https://wa.me/34911807673?text=Hola%20Alejandra%2C%20me%20interesa%20tu%20ecosistema%20digital%20con%20IA)

**📧 Contacto por email:**  
[contacto@sabenastudio.com](mailto:contacto@sabenastudio.com)

---

<div align="center">

**Construido con 💜 por Sabena Studio**

*Transformando webs en ecosistemas de crecimiento con IA y automatización*

[🌐 Visitar Sabena Studio](https://sabenastudio.com) | [📧 Contacto](mailto:contacto@sabenastudio.com) | [📱 WhatsApp](https://wa.me/34911807673)

</div>
