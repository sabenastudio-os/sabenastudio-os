# Sabena Studio - Ecosistema Digital Inteligente

[![Status](https://img.shields.io/badge/status-Production-success)](https://sabenastudio.com)
[![AI](https://img.shields.io/badge/AI-Claude%204.5%20Haiku-blueviolet)](https://www.anthropic.com/)
[![Backend](https://img.shields.io/badge/backend-Python%20%7C%20Flask-blue)](#)
[![Frontend](https://img.shields.io/badge/frontend-React%20%7C%20Vite-61dafb)](#)
[![Deploy](https://img.shields.io/badge/deploy-Railway%20%7C%20Vercel-success)](#)
[![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)

> **Ecosistema de herramientas inteligentes que automatizan la captación, cualificación y conversión de leads para Sabena Studio.**

---

## Tabla de Contenidos

**[ESPAÑOL](#español)**
- [Descripción General](#descripción-general)
- [Proyectos del Ecosistema](#proyectos-del-ecosistema)
  - [Quiz de Conversión](#1--quiz-de-conversión)
  - [Ale Bot - Asistente Virtual](#2--ale-bot---asistente-virtual-con-ia)
- [Arquitectura del Ecosistema](#arquitectura-del-ecosistema)
- [Stack Tecnológico](#stack-tecnológico)
- [Características Compartidas](#características-compartidas)
- [Casos de Uso](#casos-de-uso)
- [Métricas Clave](#métricas-clave)
- [Roadmap](#roadmap-del-ecosistema)
- [Seguridad y Privacidad](#seguridad-y-privacidad)
- [Autora](#autora)

**[ENGLISH](#english)**
- [Overview](#overview)
- [Projects](#projects)
- [Tech Stack](#tech-stack-1)
- [Key Features](#key-features)
- [Author](#author)

---

# ESPAÑOL

## Descripción General

**Sabena Studio** by Alejandra Trinca es un estudio digital que combina diseño web estratégico con inteligencia artificial aplicada. Este repositorio público documenta dos proyectos principales que demuestran la implementación práctica de IA conversacional y sistemas de scoring inteligentes para automatizar procesos comerciales.

### Propósito del Ecosistema

Ambos proyectos fueron diseñados para resolver un desafío clave de los negocios digitales modernos: **convertir visitantes web en leads cualificados sin intervención manual, operando 24/7**.

#### Problemas que Resuelve:

- ❌ **Pérdida de leads fuera de horario:** Opera 24/7 sin intervención humana
- ❌ **Tiempo perdido en consultas no cualificadas:** Evalúa automáticamente el nivel de interés
- ❌ **Fricción en el proceso de contacto:** Ofrece diagnóstico inmediato con descuentos o agendado inteligente
- ❌ **Falta de seguimiento estructurado:** Registra cada interacción con datos clave en Google Sheets
- ❌ **Comunicación no profesional:** Emails desde dominio corporativo verificado

---

## Proyectos del Ecosistema

### 1. 🎯 Quiz de Conversión

**Repositorio:** [Quiz-conversion-sabena](https://github.com/sabenastudio-os/Quiz-conversion-sabena) (Privado)

Quiz inteligente que diagnostica necesidades digitales, calcula un score personalizado y envía descuentos automáticamente.

#### Características Principales:
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

#### Flujo del Usuario:
1. Usuario responde 10 preguntas estratégicas
2. Sistema calcula score basado en necesidades y urgencia
3. Asigna descuento personalizado (15%-30%)
4. Envía email con diagnóstico + código de descuento
5. Registra lead en Google Sheets para seguimiento

---

### 2. 🤖 Ale Bot - Asistente Virtual con IA

**Repositorios:**
- Backend: [backend-ale-bot](https://github.com/sabenastudio-os/backend-ale-bot) (Privado)
- Frontend: [ale-bot-demo](https://github.com/sabenastudio-os/ale-bot-demo) (Privado)

Asistente virtual estratégico con IA integrada que cualifica leads, registra información y facilita el contacto inmediato.

#### Características Principales:
- 🧠 **IA conversacional** con Claude 4.5 Haiku
- 📊 **Lead scoring automático** durante la conversación (A/B/C)
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

#### Flujo del Usuario:
1. Usuario inicia conversación con Ale
2. Bot saluda, captura nombre y necesidad básica
3. Solicita email para envío de brief
4. Cualifica con 3-4 preguntas clave (negocio, integraciones, timeline)
5. Calcula score (A/B/C) basado en complejidad
6. Guarda lead en Google Sheets
7. Envía brief por email y ofrece WhatsApp/Email para contacto

---

## Arquitectura del Ecosistema

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

## Stack Tecnológico

### Frontend
| Tecnología | Uso | Proyectos |
|------------|-----|-----------|
| **React 18** | Framework UI | Quiz, Bot |
| **Vite 5** | Build tool & dev server | Quiz, Bot |
| **CSS Modules** | Estilos aislados | Quiz, Bot |
| **Vercel** | Hosting & CI/CD | Quiz, Bot |

### Backend
| Tecnología | Uso | Proyectos |
|------------|-----|-----------|
| **Python 3.11** | Lenguaje principal | Quiz, Bot |
| **Flask** | Web framework | Quiz, Bot |
| **Railway** | Hosting & deployment | Quiz, Bot |
| **Gunicorn** | WSGI server | Quiz, Bot |

### Inteligencia Artificial
| Tecnología | Uso | Proyectos |
|------------|-----|-----------|
| **Claude 4.5 Haiku** | LLM conversacional | Bot |
| **Anthropic SDK** | API client | Bot |
| **Function Calling** | Ejecución de acciones | Bot |

### Infraestructura y Servicios
| Tecnología | Uso | Proyectos |
|------------|-----|-----------|
| **Mailgun API** | Email transaccional | Quiz, Bot |
| **Google Sheets API** | Lead storage | Quiz, Bot |
| **Google Service Accounts** | Autenticación segura | Quiz, Bot |
| **WhatsApp Business** | Contacto directo | Quiz, Bot |

---

## Características Compartidas

### 📧 Sistema de Email Profesional
- **Remitente corporativo:** `contacto@sabenastudio.com`
- **Infraestructura:** Mailgun API con dominio verificado
- **Templates HTML:** Diseños responsivos y profesionales
- **Deliverability:** SPF + DKIM configurados
- **Deliverability rate:** 99%+

### 📊 Gestión de Leads
- **Registro automático** en Google Sheets
- **Captura completa:** nombre, email, empresa, necesidades, presupuesto, score
- **Análisis de conversión** con datos estructurados
- **Service Accounts** de Google para máxima seguridad
- **Deduplicación:** Actualiza fila si email ya existe

### 🎨 Diseño Profesional
- **UI/UX optimizado** para conversión
- **Responsive design** (mobile-first)
- **Identidad visual** coherente con Sabena Studio
- **Accesibilidad** y usabilidad prioritarias
- **Micro-interacciones** para engagement

### 🚀 Infraestructura Escalable
- **Frontend:** Vercel (deploy automático desde GitHub)
- **Backend:** Railway (escalable con 99.9% uptime)
- **Monitoreo:** Logs en tiempo real
- **CI/CD:** Despliegue automático al hacer push
- **HTTPS obligatorio** en todos los endpoints

---

## Casos de Uso

### 1. Generación de Leads Calientes 24/7
**Escenario:** Un visitante llega a las 3 AM interesado en un proyecto web.

**Solución Quiz:**
- Completa quiz en 2 minutos
- Recibe diagnóstico + descuento inmediato
- Lead registrado automáticamente con score

**Solución Bot:**
- Conversa con Ale naturalmente
- Brief personalizado enviado por email
- Opciones de contacto (WhatsApp/Email)

### 2. Cualificación Automática de Prospects
**Escenario:** 50 visitantes diarios, solo 10 son leads reales.

**Solución Quiz:**
- Sistema de scoring identifica nivel de necesidad
- Descuentos diferenciados según urgencia
- Solo leads con score >40 reciben descuentos altos

**Solución Bot:**
- IA detecta nivel de madurez del proyecto
- Score A/B/C basado en complejidad de integraciones
- Priorización automática para seguimiento

### 3. Seguimiento Estructurado
**Escenario:** Necesidad de data para decisiones comerciales.

**Solución Integrada:**
- Google Sheets con todos los leads centralizados
- Columnas estructuradas: Fecha, Nombre, Email, Negocio, Score, etc.
- Análisis de conversión y patrones de comportamiento
- Export a CRM o análisis avanzado

---

## Métricas Clave

### Rendimiento del Sistema

| Métrica | Quiz | Bot Ale |
|---------|------|---------|
| **Tiempo de respuesta** | ~1-2s | ~2-3s |
| **Disponibilidad** | 24/7 | 24/7 |
| **Idiomas soportados** | ES / EN | ES / EN |
| **Costo por interacción** | ~$0.02 | ~$0.05-0.10 |
| **Email deliverability** | 99%+ | 99%+ |
| **Tasa de completado** | ~75% | ~85% |

### Impacto en el Negocio

- ⏰ **Tiempo ahorrado:** ~10 horas/semana en cualificación manual
- 📈 **Aumento de conversión:** 40% más leads cualificados
- 🎯 **Mejor segmentación:** Score A/B/C permite priorización efectiva
- 📊 **Data estructurada:** 100% de interacciones registradas para análisis

---

## Roadmap del Ecosistema

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
- [ ] Multi-idioma (Portugués, Francés)

### 🔮 Futuro (v2.0)
- [ ] Integración con CRM (HubSpot / Notion)
- [ ] Lead scoring con Machine Learning
- [ ] Automatización de onboarding de clientes
- [ ] Integración con redes sociales (LinkedIn, Instagram)
- [ ] API pública para integraciones de terceros
- [ ] Panel de analytics en tiempo real

---

## Seguridad y Privacidad

### Medidas Implementadas

- ✅ **Credenciales encriptadas** en variables de entorno
- ✅ **HTTPS obligatorio** en todos los endpoints
- ✅ **CORS configurado** para dominios autorizados únicamente
- ✅ **Service Accounts de Google** con permisos mínimos necesarios
- ✅ **No almacenamiento de datos sensibles** en servidores
- ✅ **Emails desde dominio verificado** (SPF + DKIM)
- ✅ **Google Workspace** para gestión corporativa de emails

### Compliance

- ⚠️ **GDPR:** En revisión (pendiente para operación completa en Europa)
- ✅ **Encriptación en tránsito:** TLS 1.3
- ✅ **Autenticación API:** Keys rotables
- ✅ **Logs auditables:** Railway + Vercel

---

## Instalación y Desarrollo

### Prerrequisitos
- Node.js 18+
- Python 3.11+
- Cuenta de Anthropic (Claude API)
- Cuenta de Mailgun
- Google Cloud Project con Sheets API habilitada

### Clonar Repositorios

```bash
# Quiz (privado - requiere acceso)
git clone https://github.com/sabenastudio-os/Quiz-conversion-sabena.git

# Bot Backend (privado - requiere acceso)
git clone https://github.com/sabenastudio-os/backend-ale-bot.git

# Bot Frontend (privado - requiere acceso)
git clone https://github.com/sabenastudio-os/ale-bot-demo.git

# Ecosistema (público)
git clone https://github.com/sabenastudio-os/sabenastudio-ecosystem.git
```

### Configuración

Cada proyecto incluye:
- `.env.example` - Template de variables de entorno
- `README.md` - Documentación específica del proyecto
- Instrucciones de deploy para Railway/Vercel

---

## Licencia

Todos los proyectos del ecosistema Sabena Studio utilizan la Licencia MIT.

**Copyright (c) 2025 Sabena Studio by Alejandra Trinca**

Ver archivos LICENSE en cada repositorio para más detalles.

---

## Autora

**Alejandra Trinca**  
Framer Expert Certificada | Desarrollo Web con IA | Automatización Inteligente

- 🌐 Web: [sabenastudio.com](https://sabenastudio.com)
- 📧 Email: [contacto@sabenastudio.com](mailto:contacto@sabenastudio.com)
- 💼 LinkedIn: [linkedin.com/in/alejandra-trinca](https://linkedin.com/in/alejandra-trinca)
- 📱 WhatsApp: [+34 911 807 673](https://wa.me/34911807673)

### Sobre Sabena Studio

Sabena Studio no es una agencia tradicional. Es el estudio digital de Alejandra Trinca, donde más de 20 años de experiencia ejecutiva se fusionan con tecnología de vanguardia. Cada proyecto combina estrategia, diseño y desarrollo asistido por IA para crear ecosistemas digitales que generan resultados medibles.

**Especialidades:**
- Webs inteligentes en Framer, Wix, Durable, Squarespace
- Integración de IA conversacional (chatbots, quizzes, sistemas personalizados)
- Desarrollos custom con React + Flask + APIs
- Automatización de procesos comerciales
- Optimización basada en datos (Analytics + Clarity)

---

## Agradecimientos

- [Anthropic](https://www.anthropic.com/) - Claude AI para asistencia con IA
- [Mailgun](https://www.mailgun.com/) - Infraestructura de email transaccional
- [Railway](https://railway.app/) - Hosting del backend
- [Vercel](https://vercel.com/) - Hosting del frontend
- [Google Cloud](https://cloud.google.com/) - APIs de productividad (Sheets, Workspace)

---

## Contacto y Soporte

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

---
---

# ENGLISH

## Overview

**Sabena Studio** by Alejandra Trinca is a digital studio that combines strategic web design with applied artificial intelligence. This public repository documents two main projects demonstrating practical implementation of conversational AI and intelligent scoring systems to automate business processes.

Both projects solve a key challenge for modern digital businesses: **converting website visitors into qualified leads without manual intervention, operating 24/7**.

---

## Projects

### Conversion Quiz
**Repository:** [Quiz-conversion-sabena](https://github.com/sabenastudio-os/Quiz-conversion-sabena) (Private)

Intelligent quiz that diagnoses digital needs, calculates personalized scores, and automatically sends discounts.

**Key Features:**
- Intelligent scoring system (20-100 points)
- Personalized discounts (15%, 25%, 30%)
- Automated emails via Mailgun from `contacto@sabenastudio.com`
- Automatic registration in Google Sheets
- Bilingual interface (ES/EN)

**Tech Stack:** React + Vite (Vercel) | Flask + Python (Railway) | Mailgun API | Google Sheets API

---

### Ale Bot - Virtual Assistant
**Repositories:** [backend-ale-bot](https://github.com/sabenastudio-os/backend-ale-bot) | [ale-bot-demo](https://github.com/sabenastudio-os/ale-bot-demo) (Private)

Strategic virtual assistant with integrated AI that qualifies leads and facilitates immediate contact.

**Key Features:**
- Conversational AI with Claude 4.5 Haiku
- Automatic lead scoring (A/B/C)
- Brief sending via Mailgun
- WhatsApp integration
- Embeddable responsive widget

**Tech Stack:** React 18 + Vite (Vercel) | Flask + Python (Railway) | Anthropic Claude API | Mailgun API | Google Sheets API

---

## Tech Stack

### Core Technologies
- **Frontend:** React 18, Vite 5, CSS Modules
- **Backend:** Python 3.11, Flask, Gunicorn
- **AI:** Anthropic Claude 4.5 Haiku with Function Calling
- **Email:** Mailgun API
- **Storage:** Google Sheets API
- **Hosting:** Vercel (frontend), Railway (backend)

### Key Integrations
- Google Service Accounts (secure authentication)
- WhatsApp Business (direct contact)
- Google Workspace (corporate email management)

---

## Key Features

### Professional Email System
- Corporate sender: `contacto@sabenastudio.com`
- Mailgun infrastructure with verified domain
- Responsive HTML templates
- 99%+ deliverability rate

### Lead Management
- Automatic registration in Google Sheets
- Complete capture: name, email, business, needs, budget, score
- Deduplication: updates row if email exists
- Structured data for analysis

### Scalable Infrastructure
- Automatic deployment from GitHub
- 24/7 availability
- Real-time logs
- HTTPS mandatory on all endpoints

---

## Metrics

| Metric | Quiz | Bot |
|--------|------|-----|
| Response time | ~1-2s | ~2-3s |
| Availability | 24/7 | 24/7 |
| Languages | ES/EN | ES/EN |
| Cost per interaction | ~$0.02 | ~$0.05-0.10 |
| Email deliverability | 99%+ | 99%+ |

---

## Use Cases

**1. 24/7 Lead Generation**
- Visitors converted into qualified leads at any time
- Immediate response with diagnosis + discount (Quiz)
- Natural conversation + personalized brief (Bot)

**2. Automatic Prospect Qualification**
- Intelligent scoring system identifies need level
- A/B/C score based on integration complexity
- Automatic prioritization for follow-up

**3. Structured Follow-up**
- Centralized leads in Google Sheets
- Structured data for business decisions
- Export to CRM or advanced analysis

---

## Security & Privacy

- Encrypted credentials in environment variables
- HTTPS mandatory on all endpoints
- CORS configured for authorized domains only
- Google Service Accounts with minimum necessary permissions
- No sensitive data storage on servers
- Emails from verified domain (SPF + DKIM)

---

## License

All Sabena Studio ecosystem projects use the MIT License.

**Copyright (c) 2025 Sabena Studio by Alejandra Trinca**

See LICENSE files in each repository for details.

---

## Author

**Alejandra Trinca**  
Certified Framer Expert | Web Development with AI | Intelligent Automation

- Web: [sabenastudio.com](https://sabenastudio.com)
- Email: [contacto@sabenastudio.com](mailto:contacto@sabenastudio.com)
- LinkedIn: [linkedin.com/in/alejandra-trinca](https://linkedin.com/in/alejandra-trinca)
- WhatsApp: [+34 911 807 673](https://wa.me/34911807673)

### About Sabena Studio

Sabena Studio is not a traditional agency. It's Alejandra Trinca's digital studio, where over 20 years of executive experience merge with cutting-edge technology. Each project combines strategy, design, and AI-assisted development to create digital ecosystems that generate measurable results.

---

## Contact

Interested in implementing similar solutions for your business?

**WhatsApp:** [Send message](https://wa.me/34911807673?text=Hello%20Alejandra%2C%20I'm%20interested%20in%20your%20AI-powered%20digital%20ecosystem)

**Email:** [contacto@sabenastudio.com](mailto:contacto@sabenastudio.com)

---

<div align="center">

**Built with love by Sabena Studio**

*Transforming websites into growth ecosystems with AI and automation*

[Visit Sabena Studio](https://sabenastudio.com) | [Contact](mailto:contacto@sabenastudio.com) | [WhatsApp](https://wa.me/34911807673)

</div>
