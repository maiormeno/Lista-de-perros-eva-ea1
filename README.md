# Lista de perros 🐶

Este repositorio contiene la base del trabajo para el pipeline de DevOps


## 🌳 Estrategia de ramificación

> ✏Como equipo optamos por la estrategia **GitFlow**
> 
> Porque GitFlow nos permite separar el desarrollo de nuevas características en ramas 'feature/' y el aislamiento de correcciones en ramas 'hotfix/'. La rama 'develop' actúa como centro de integración constante antes de fusionar los cambios a 'main'. Esto es ideal para controlar en Java.

---

## 📝 Convenciones de commits

> ✏Decidimos utilizar el estándar **Conventional Commits**
> 
> 'feat:' para incorporar nuevas funcionalidades en Java (por ejemplo, 'feat(perro): agregar endpoint de lista de razas').

> 'fix:' para solucionar errores del código (por ejemplo, 'fix(servicio): corregir exception NullPointer en controlador').

> 'docs:' para cambios exclusivos de la documentación

> 'style:' para formatear sin cambios en la lógica del negocio.

---

## 🔀 Convenciones de naming de ramas

> ✏Definimos que para nombrar nuestras ramas deben ser descriptivas y estructuradas para identificar rápido el propósito y cambios.
> 
> Utilizamos prefijos claros basados en GitFlow acompañados de una descripción, facilitando la trazabilidad del código y evitando conflictos en entornos colaborativos.
> 
> **'main'**: Muestra la versión de producción, estable y lista para utilizarse.
> 
> **'develop'**: Es la rama principal donde se integra todo continuamente y se aprecian los nuevos avances.
> 
> **'feature/<>'**: Será utilizada para nuevas funcionalidades, como agregar validación de perros o actualizar la interfaz de la lista.
> 
> **'hotfix/<>'**: Es exclusiva para soluciones urgentes de errores detectados en ('main').
---

## 🔍 Estrategia de revisión (Pull Requests)

> ✏ Para la calidad e integridad del código, establecimos estos requisitos:
> - Ningún cambio ingresa directamente a 'main' y/o 'develop'.
> - Cada cambio requiere la apertura de un **Pull Request**.
> - Se revisa el código entre los integrantes.
> - En la fusión, el pipeline de **Github Actions** debe ejecutarse sin fallas.


---

## ⚙️ Automatización (CI/CD)

> ✏️ Configuramos un flujo de integración continua (CI) a través de **Github Actions**
> 
> -**Triggers:** Se activan en cada 'push' hacia 'develop' y con cada 'pull_request' a 'main'.
> 
> -**Acciones:** Configuran el entorno de Java y descarga las dependencias con Maven.

---

## 📁 Estructura de carpetas

```
Lista-de-perros/
├── .github/
│   └── workflows/
│       └── ci.yml
├── index.html
├── index.js
├── style.css
└── README.md
```
---

## 👥 Autores

- Integrante 1 — Maira Ormeño
- Integrante 2 — Michelle Serrano
- Integrante 3 — Valentina Ruiz

*Proyecto original: repaso de conexión a API y manejo de eventos en JavaScript. Adaptado como base para la Evaluación Parcial N°1, DOY0101 — Ingeniería DevOps.*
