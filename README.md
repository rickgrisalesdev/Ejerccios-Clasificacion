<div align="center">

![Estud-IA Logo](./Estud-IA_Logo.png)

# **Campus Estud-IA**

# 🌸 Clasificación de Flores Iris - Machine Learning

### Proyecto de la Universidad Estud-IA
**Ejercicio #1 - Clasificación Supervisada**

</div>

## 📋 Tabla de Contenidos
1. [Descripción del Proyecto](#descripción-del-proyecto)
2. [¿Qué se quiere conseguir?](#qué-se-quiere-conseguir)
3. [Requisitos Previos](#requisitos-previos)
4. [Configuración del Entorno Virtual](#configuración-del-entorno-virtual)
5. [Instalación de Dependencias](#instalación-de-dependencias)
6. [Cómo ejecutar el Proyecto](#cómo-ejecutar-el-proyecto)
7. [Entendiendo el Código](#entendiendo-el-código)

---

## 📚 Descripción del Proyecto

Este proyecto implementa un **modelo de Machine Learning de clasificación supervisada** usando el famoso dataset Iris. 

El objetivo es **predecir qué tipo de flor es** (Setosa, Versicolor o Virginica) basándose en características físicas como:
- Largo del sépalo
- Ancho del sépalo
- Largo del pétalo
- Ancho del pétalo

---

## 🎯 ¿Qué se quiere conseguir?

Este proyecto cumple con los siguientes objetivos educativos:

✅ **Aprender Machine Learning**: Entender cómo funcionan los modelos de clasificación

✅ **Procesamiento de datos**: Cargar, analizar y preparar datos

✅ **Visualización**: Crear gráficos para entender los datos

✅ **Entrenamiento de modelos**: Usar el algoritmo Random Forest

✅ **Evaluación**: Medir qué tan bien funciona el modelo

✅ **Predicciones**: Usar el modelo entrenado para predecir nuevas flores

---

## 🔧 Requisitos Previos

Antes de comenzar, necesitas tener instalado en tu computadora:

### Python
- **Python 3.8 o superior**
- Puedes descargarlo desde: https://www.python.org/downloads/

**¿Cómo verificar si tienes Python?**
```bash
python --version
```

Si ves algo como `Python 3.10.5`, significa que ya tienes Python instalado.

---

## 🚀 Configuración del Entorno Virtual

Un **entorno virtual** es como una carpeta especial que guarda todas las librerías de tu proyecto, separadas del resto de tu computadora. Esto es muy importante para no contaminar tu sistema.

### Paso 1: Abre la terminal/CMD

**En Windows:**
- Presiona `Win + R`
- Escribe `cmd` y presiona Enter

**En Mac/Linux:**
- Abre la Terminal (busca en Aplicaciones)

### Paso 2: Navega a la carpeta del proyecto

```bash
cd ruta/a/tu/proyecto
```

Por ejemplo:
```bash
cd /home/mendozalz/Escritorio/StudiaIA/Ejercicio#1-clasificacion
```

### Paso 3: Crea el entorno virtual

**En Windows:**
```bash
python -m venv .venv
```

**En Mac/Linux:**
```bash
python3 -m venv .venv
```

Este comando crea una carpeta llamada `venv` (es como un "mini Python" solo para tu proyecto).

### Paso 4: Activa el entorno virtual

**En Windows:**
```bash
venv\Scripts\activate
```

**En Mac/Linux:**
```bash
source venv/bin/activate
```

**¿Funcionó?** Si ves algo como esto en tu terminal, significa que los pasos anteriores fueron correctos:
```bash
(venv) $
```

Nota que ahora tu terminal muestra `(venv)` al inicio. Eso significa que estás dentro del entorno virtual.

---

## 📦 Instalación de Dependencias

Las **dependencias** son librerías externas (código escrito por otros colaboradores) que nuestro proyecto necesita para funcionar.

### Paso 1: Asegúrate de tener el archivo `requirements.txt`

El archivo `requirements.txt` debe estar en la carpeta de tu proyecto junto a `app.py`.

### Paso 2: Instala todas las dependencias

Con el entorno virtual activado (recuerda que debe mostrar `(venv)` en tu terminal), ejecuta:

```bash
pip install -r requirements.txt
```

### ¿Qué hace este comando?

- `pip` = el gestor de paquetes de Python (es como un "instalador" de librerías)
- `install` = instalar
- `-r requirements.txt` = lee el archivo requirements.txt y instala todo lo que dice

**Espera un momento** mientras todas las librerías se descargan e instalan. Verás algo como:
```
Successfully installed numpy-1.24.0 pandas-2.0.0 ...
```

### Actualizar una dependencia (opcional)

Si en el futuro necesitas actualizar una librería específica:

```bash
pip install --upgrade nombre_libreria
```

Por ejemplo:
```bash
pip install --upgrade pandas
```

---

## ▶️ Cómo ejecutar el Proyecto

### Paso 1: Asegúrate de estar en el entorno virtual

Tu terminal debe mostrar `(venv)` al inicio:
```bash
(venv) $
```

### Paso 2: Ejecuta el archivo principal

```bash
python app.py
```

### ¿Qué pasará?

El programa hará esto automáticamente:

1. 📊 **Carga el dataset Iris** - Descarga 150 flores con sus características
2. 📈 **Crea visualizaciones** - Muestra gráficos para entender los datos
3. 🧠 **Entrena el modelo** - Usa Random Forest para aprender patrones
4. ✅ **Evalúa el resultado** - Muestra qué tan preciso es el modelo
5. 🔮 **Hace predicciones** - Prueba el modelo con nuevas flores

Deberías ver algo como:
```
============================================================
DEMOSTRACION: CLASIFICACION SUPERVISADA - IRIS
============================================================
Cargando dataset Iris...
Dataset cargado: 150 muestras, 4 características
...
Accuracy general: 1.0000 (100.00%)
```

---

## 💡 Entendiendo el Código

### Estructura del Proyecto

```
Ejercicio#1-clasificacion/
│
├── app.py                  # Archivo principal (el código del proyecto)
├── requirements.txt        # Lista de dependencias
└── README.md              # Este archivo (instrucciones)
```

### Las Librerías Explicadas

| Librería | Para qué sirve |
|----------|---|
| **numpy** | Trabajo con números y arrays (listas de números) |
| **pandas** | Manejo de datos en tablas (como Excel en Python) |
| **matplotlib** | Crear gráficos y visualizaciones |
| **seaborn** | Gráficos más bonitos y complejos que matplotlib |
| **scikit-learn** | Modelos de Machine Learning listos para usar |

### Flujo del Programa

```
1. Cargar datos Iris (150 flores)
           ↓
2. Visualizar datos (crear gráficos)
           ↓
3. Dividir datos en entrenamiento (80%) y prueba (20%)
           ↓
4. Normalizar datos (hacer que todos tengan la misma escala)
           ↓
5. Entrenar modelo Random Forest
           ↓
6. Evaluar el modelo
           ↓
7. Hacer predicciones con nuevas flores
```

---

## 🆘 Solución de Problemas

### Problema: "Python no se reconoce"

**Solución:** Python no está en el PATH de tu sistema. Reinstálalo asegurándote de marcar la opción "Add Python to PATH".

### Problema: "No existe el archivo requirements.txt"

**Solución:** Asegúrate de que el archivo `requirements.txt` está en la misma carpeta que `app.py`.

### Problema: "ModuleNotFoundError: No module named 'sklearn'"

**Solución:** Las dependencias no se instalaron correctamente. Intenta:
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

### Problema: "No puedo activar el entorno virtual"

**Solución:** Verifica que estés en la carpeta correcta del proyecto y usa el comando correcto para tu sistema operativo.

---

## 📖 Recursos Adicionales

- [Documentación oficial de scikit-learn](https://scikit-learn.org/)
- [Documentación de pandas](https://pandas.pydata.org/)
- [Dataset Iris en Kaggle](https://www.kaggle.com/datasets/uciml/iris)
- [Tutorial de Random Forest](https://medium.com/@evertongomede/understanding-random-forest-classifier-e066f2e0b2ef)

---

## 📝 Lo que Aprendiste

Después de completar este proyecto, ahora sabes:

✅ Cómo crear un entorno virtual
✅ Cómo instalar dependencias de Python
✅ Cómo cargar y explorar datasets
✅ Cómo preprocesar datos
✅ Cómo entrenar un modelo de Machine Learning
✅ Cómo evaluar modelos
✅ Cómo hacer predicciones

¡Felicidades! 🎉 Ya has completado tu primer proyecto de Machine Learning.

---

**Última actualización:** 19 de febrero de 2026
