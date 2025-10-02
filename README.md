# Laboratorio SQL Injection - Análisis de Vulnerabilidades

> Entrega: actividad de ciberseguridad (SQL Injection)  
> Archivo base: `ciberseguridad-actividad01.md` — versión entregada: 2025-09-26

---

## Información del Equipo
- **Integrante 1:** Juan Fernando Bueno Torres — `@JuanFer2004`  
- **Fecha:** 2025-09-26

**Distribución de responsabilidades**
- Integrante 1: Todo.  

**Repositorio de trabajo / entrega**  
- Fork / desarrollo: `https://github.com/JuanFer2004/sql-injection-lab`  
- Repositorio final de entrega: `https://github.com/JuanFer2004/Trabajo` 

---

## Tabla de Contenidos
1. [Instalación y Configuración](#1-instalación-y-configuración)  
2. [Vulnerabilidades Identificadas](#2-vulnerabilidades-identificadas)  
   - [2.1 Login Bypass](#21-login-bypass)  
   - [2.2 Union-Based Injection](#22-union-based-injection)  
   - [2.3 Blind SQL Injection](#23-blind-sql-injection)  
3. [Técnicas de Explotación y Evidencias](#3-técnicas-de-explotación-y-evidencias)  
4. [Análisis de Impacto y Contramedidas](#4-análisis-de-impacto-y-contramedidas)  
5. [Reflexión Ética del Equipo](#5-reflexión-ética-del-equipo)  
6. [Apéndices: Payloads, Comandos y Troubleshooting](#6-apéndices-payloads-comandos-y-troubleshooting)  
7. [Checklist de Entrega](#7-checklist-de-entrega)

---

## 1. Instalación y Configuración

### Requisitos
- Python 3.8+  
- Git  
- (Opcional) `uvicorn` si la app usa FastAPI  
- Sistema: Windows / Linux / macOS

### Clonar el repositorio
```bash
# Clonar el repo de entrega (ajusta la URL si entregas en otro repo)
git clone https://github.com/JuanFer2004/Trabajo.git
cd ciberseguridad
