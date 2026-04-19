# Arquitectura de Software (Resumen básico)

## ¿Qué es la arquitectura de software?

Es el conjunto de decisiones sobre la estructura de un sistema (componentes, relaciones y responsabilidades).  
Define cómo se comunican las partes y cómo evolucionará el sistema, permitiendo que sea escalable, mantenible y entendible en el tiempo.

---

## 🗂️ 1. Arquitectura de Repositorio (Dónde guardas el código)

### Monorepo

Un solo repositorio que contiene múltiples proyectos o partes del sistema (frontend, backend, etc).

**Cuándo usar:**

- Equipos pequeños o desarrolladores individuales
- Commits sincronizados (frontend + backend juntos)
- Todo centralizado en un solo lugar

---

### Polyrepo / Multirepo

Múltiples repositorios separados (por ejemplo, uno para backend y otro para frontend).

**Cuándo usar:**

- Equipos separados
- Proyectos independientes

---

## 2. Arquitectura de Sistema (Cómo funciona en internet)

### Monolítica

Toda la aplicación está en un solo sistema que maneja todas las funcionalidades.

---

### Microservicios

El backend se divide en varios servicios (ej: productos, carrito, usuarios), que se comunican entre sí.

---

## 3. Arquitectura de Código Interna (Organización interna)

### Arquitectura en Capas

La información viaja por capas:  
**Ruta → Controlador → Servicio → Base de Datos**  
Cada capa tiene una responsabilidad específica.

---

### MVC (Modelo - Vista - Controlador)

- **Modelo:** Datos y lógica de negocio
- **Vista:** Lo que ve el usuario (HTML/React)
- **Controlador:** Conecta modelo y vista

---

### Clean Architecture

Se diseña como una cebolla desde el núcleo hacia lo externo.  
Las capas externas dependen de las internas, lo que permite cambiar capas externas sin modificar el núcleo.

---

## Objetivo

Este documento es un resumen simple para entender los conceptos básicos de arquitectura de software.
