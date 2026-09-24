# Laboratorio 01: Fundamentos de IA y Agente Reactivo

**Curso:** IS484 - Inteligencia Artificial  
**Universidad:** Universidad Nacional de San Cristóbal de Huamanga (UNSCH)  
**Estudiante:** [Tu Nombre y Apellidos]  
**Semestre:** [Ej. 2025-I]

---

## 📌 Descripción del Laboratorio

Este repositorio contiene el desarrollo del **Laboratorio 01**, el cual tiene como objetivos:
- Clasificar sistemas de Inteligencia Artificial según el tipo de problema y área de aplicación.
- Representar sistemas de IA mediante el esquema formal de agente inteligente (PEAS).
- Configurar un entorno de trabajo en Python con Jupyter Notebook.
- Implementar un agente reactivo simple (termostato) y un agente de riego como extensión.

---

## 📂 Contenido del Repositorio

- `IS484_Lab01_Apellido.ipynb`: Notebook principal con las actividades desarrolladas.
- `README.md`: Este archivo con la documentación del laboratorio.
- `extensión/` (opcional): Carpeta con el código adicional del agente de riego.

---

## 🛠️ Tecnologías y Herramientas Utilizadas

- Python 3.x
- Jupyter Notebook
- NumPy, Pandas, Matplotlib, Scikit-learn, SciPy
- Git y GitHub Classroom

---

## ✅ Actividades Completadas

### 1. Verificación del Entorno
- [x] Instalación de Python y verificación de versión.
- [x] Creación de entorno virtual e instalación de bibliotecas.
- [x] Verificación funcional con un sistema anti-fraude simulado.

### 2. Clasificación de Sistemas de IA
Se analizaron dos sistemas:
| Sistema | Entrada | Salida | Tipo de Problema | Área de IA |
|---------|---------|--------|------------------|------------|
| Filtro anti-spam de Gmail | Correo electrónico | Spam / No spam | Clasificación | Procesamiento de Lenguaje Natural (NLP) |
| Sistema de recomendación de Netflix | Historial de usuario | Lista de películas | Recomendación | Sistemas de Recomendación |

### 3. Representación PEAS (Sistema Anti-Fraude Bancario)
- **Percepción (S):** Hora, monto, ubicación, historial de transacciones.
- **Acciones (A):** Aprobar, rechazar, solicitar verificación adicional.
- **Entorno (E):** Red bancaria en tiempo real.
- **Objetivo:** Detectar y prevenir fraudes.
- **Medida de Desempeño (P):** Tasa de fraude detectado vs. falsos positivos.
- **Tipo de Agente:** Basado en modelos y aprendizaje.
- **Racionalidad:** Sí, porque maximiza la detección de fraudes minimizando errores.
- **IA:** Estrecha (especializada en fraude).

### 4. Agente Reactivo Simple: Termostato
- **Percepción:** Temperatura actual.
- **Acciones:** Encender calefacción, apagar, encender aire acondicionado.
- **Entorno:** Habitación.
- **Objetivo:** Mantener temperatura en 22°C.
- **Medida de Desempeño:** Confort térmico y eficiencia energética.

**Reglas de decisión:**
- Si `temp > 23°C` → Encender A/C.
- Si `temp < 21°C` → Encender calefacción.
- Si `21°C ≤ temp ≤ 23°C` → Apagar todo.

### 5. Extensión: Agente de Riego Automático
- **Percepción:** Humedad del suelo, pronóstico de lluvia.
- **Acciones:** Regar, no regar.
- **Entorno:** Jardín.
- **Objetivo:** Mantener humedad óptima sin desperdiciar agua.
- **Medida de Desempeño:** Salud de las plantas y ahorro de agua.

**Reglas:**
- Si `humedad < 30` y `no lloverá` → Regar.
- Si `humedad < 30` y `lloverá` → No regar (esperar lluvia).
- Si `humedad ≥ 30` → No regar.

---

## 🚀 Cómo Ejecutar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/Henrixrs/LAB_1_IA.git
