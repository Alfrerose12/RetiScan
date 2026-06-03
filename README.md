# RetiScan

![Status](https://img.shields.io/badge/Status-In__Development-orange?style=flat-for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Multiplatform__PWA-blue?style=flat-for-the-badge)
![Framework](https://img.shields.io/badge/Frontend-Flutter-02569B?style=flat-for-the-badge&logo=flutter)
![Backend](https://img.shields.io/badge/Backend-Node.js__%2F__Express-339933?style=flat-for-the-badge&logo=node.js)
![AI-Engine](https://img.shields.io/badge/AI__Engine-Python__%2F__Flask-000000?style=flat-for-the-badge&logo=python)

> **RetiScan** es un ecosistema digital multiplataforma y de grado médico diseñado para la detección temprana de retinopatía diabética mediante la implementación de modelos avanzados de Inteligencia Artificial (Redes Neuronales Convolucionales) y el procesamiento asíncrono de imágenes de fondo de ojo.

---

## 🚀 Características Principales

* **Pipeline de IA Asíncrono:** Procesamiento no bloqueante de imágenes diagnósticas utilizando una arquitectura basada en eventos (Estatus: `PENDING` ➡️ `PROCESSING` ➡️ `COMPLETED`).
* **Seguridad de Grado Clínico:** Autenticación robusta de dos factores (MFA - OTP) para el acceso seguro de pacientes y médicos.
* **Control de Acceso Basado en Roles (RBAC):** Middleware dedicado para segmentar permisos de manera estricta entre el personal médico (`MEDICO`) y los usuarios finales (`PACIENTE`).
* **Aislamiento de Datos (Multi-tenancy):** Capa de seguridad que garantiza el aislamiento completo de los expedientes clínicos, asegurando que los médicos solo tengan visibilidad sobre sus pacientes asignados.
* **Gobernanza B2B:** Control integrado de acceso premium y validación de vigencia de licenciamiento mediante middleware de suscripción verificado.

---

## 🏗️ Arquitectura del Sistema (Por Capas)

El proyecto se rige bajo un diseño desacoplado y distribuido en tres capas principales operando de forma independiente:

1. **Capa de Presentación (Frontend):** Aplicación Web Progresiva (PWA) de alta fidelidad construida en **Flutter**, optimizada para la captura ágil de imágenes y la visualización interactiva de reportes clínicos.
2. **Capa de Negocio y Orquestación (Backend Core):** API RESTful desarrollada en **Node.js** con **Express**, encargada de la autenticación JWT, rate limiting, validación de esquemas y la gestión del expediente clínico en base de datos.
3. **Capa Analítica (AI Engine):** Microservicio especializado en **Python** con **Flask** que expone el pipeline analítico de la red neuronal ResNet-50 optimizada para clasificación de patologías retinianas.

---

## 🛠️ Stack Tecnológico

* **Frontend:** Flutter (Dart) para distribución PWA y Mobile.
* **Backend:** Node.js, Express.js, TypeScript.
* **Procesamiento de IA:** Python, Flask, TensorFlow / Keras (ResNet-50).
* **Persistencia de Datos:** PostgreSQL (Expedientes clínicos) y MongoDB (Logs de auditoría del pipeline).
* **Infraestructura:** Docker y Docker Compose para la containerización y homogeneidad del entorno.

---

## 🔧 Inicialización del Entorno de Desarrollo

### Prerrequisitos
* Docker Desktop o Docker Engine (v26.x+)
* Docker Compose
* Git

### Despliegue Rápido
1. Clonar el repositorio principal:
```bash
   git clone [https://github.com/Alfrerose12/RetiScan.git](https://github.com/Alfrerose12/RetiScan.git)
   cd RetiScan