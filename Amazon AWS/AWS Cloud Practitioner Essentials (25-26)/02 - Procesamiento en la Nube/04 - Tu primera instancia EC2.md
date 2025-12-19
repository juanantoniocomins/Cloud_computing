# 🚀 ¡Tu Primera Instancia EC2! - Del Cero al Servidor Web en Minutos

> 🎯 **Lo que vas a aprender:**
> - Cómo lanzar una instancia EC2 paso a paso
> - Las configuraciones clave que necesitas
> - Qué es una AMI y por qué es importante
> - Cómo crear un servidor web funcional ¡YA!

---

## 🎬 ¡Es Hora de la Acción!

Has aprendido mucho sobre EC2... ahora viene lo mejor:

```
💭 "¿Cómo puedo crear una instancia de EC2?"
```

### 🎯 ¡Vamos a verlo en ACCIÓN!

```
    📖 Teoría ✅ (Ya la sabes)
        ↓
    🎬 PRÁCTICA ← ¡AQUÍ ESTAMOS!
        ↓
    🚀 Tu servidor web funcionando
```

---

## 🎮 La Misión de Hoy

### 🎯 Objetivo

```
Crear un SERVIDOR WEB completamente funcional
    usando Amazon EC2
    en MINUTOS
    
🖥️ → ☁️ → 🌐 → ✅
```

**Al final de esta demostración:**
- ✅ Tendrás una instancia de EC2 funcionando
- ✅ Con un servidor web activo
- ✅ Accesible desde internet
- ✅ ¡Todo creado por TI!

---

## 🛠️ Paso a Paso: Lanzar Tu Instancia EC2

### 📋 Resumen del proceso

```
1️⃣ Ir a la Consola de EC2
2️⃣ Elegir nombre
3️⃣ Seleccionar AMI (plantilla)
4️⃣ Elegir tipo de instancia
5️⃣ Configurar par de claves
6️⃣ Ajustar red
7️⃣ Configurar almacenamiento
8️⃣ Añadir script de datos de usuario
9️⃣ ¡LANZAR!
🎉 Servidor web funcionando
```

---

## 1️⃣ Paso 1: Ir a la Consola de EC2

### 🌐 Accede a la consola

```
Opciones para encontrar EC2:
    
    📌 Sección "Visitados recientemente"
    ⭐ Barra de atajos
    🔍 Buscar "EC2" en la barra de búsqueda
    
    → Click en el servicio EC2
```

### 🎯 Una vez dentro

```
Verás MUCHÍSIMAS opciones... 😱
    
Pero nos centraremos en:
    🚀 "Lanzar instancia" (Launch Instance)
    
    ← ¡Ese botón es el que necesitas!
```

---

## 2️⃣ Paso 2: Elegir un Nombre

### 📛 Dale identidad a tu instancia

```
¿Por qué necesitas un nombre?
    🔍 Para poder encontrarla más tarde
    📋 Para identificarla entre muchas
    🎯 Para organizarte mejor
    
Ejemplo:
    "mi-primer-servidor-web"
    "servidor-web-prueba"
    "web-server-demo"
```

---

## 3️⃣ Paso 3: Elegir la AMI

### 🖼️ ¿Qué es una AMI?

**AMI = Amazon Machine Image (Imagen de Máquina de Amazon)**

```
AMI:
    📦 Plantilla del sistema operativo
    🛠️ Aplicaciones integradas incluidas
    🎨 Configuración predefinida
    ⚡ Lista para usar
    
    = "La receta de tu servidor" 👨‍🍳
```

### 🎯 Para esta demo: Amazon Linux

```
Amazon Linux AMI:
    🐧 Basada en Linux
    🌐 Ideal para servidor web de uso general
    ✅ Gratuita
    🚀 Optimizada para AWS
    
    = Perfecta para empezar
```

### 💡 AMIs son plantillas prediseñadas

> **Las AMI son imágenes de máquina virtual prediseñadas que tienen los componentes básicos necesarios para iniciar una instancia.**

```
AMI contiene:
    💻 Sistema operativo base
    📦 Software preinstalado
    ⚙️ Configuraciones iniciales
    
Sin AMI → Configurar TODO manualmente 😓
Con AMI → ¡Listo en segundos! ⚡
```

---

## 4️⃣ Paso 4: Elegir el Tipo de Instancia

### 💪 ¿Cuánta potencia necesitas?

```
Tipo de instancia:
    💻 Define la potencia de computación
    🧠 CPU y memoria
    📊 Recursos del servidor
```

### 🎯 Para esta demo: t2.micro

```
t2.micro:
    🐭 Instancia básica (pequeña)
    💻 1 CPU virtual (vCPU)
    🧠 1 GB de memoria RAM
    💚 Nivel GRATUITO ← ¡GRATIS!
    
Especificaciones:
    ┌─────────────────────┐
    │  t2.micro           │
    │  ─────────          │
    │  💻 1 vCPU          │
    │  🧠 1 GB RAM        │
    │  💰 FREE TIER ✅    │
    └─────────────────────┘
    
    = Perfecto para aprender sin gastar
```

---

## 5️⃣ Paso 5: Configurar Par de Claves

### 🔐 Tu llave de acceso

```
Par de claves:
    🔑 Clave PÚBLICA → Va a la instancia EC2
    🔐 Clave PRIVADA → TÚ la guardas
    
¿Para qué?
    🚪 Para iniciar sesión en tu instancia
    🛡️ Seguridad de acceso
```

### 🎯 ¿Qué es exactamente?

**Un par de claves es exactamente eso:**
- 🔓 **Clave pública:** Se introduce en la instancia de EC2
- 🔒 **Clave privada:** La conservas tú (¡nunca la compartas!)

### 💡 En la demo

```
Opciones:
    ✅ Crear un par de claves nuevo
    ✅ Elegir una clave que ya tengas
    
Para esta demo:
    → Elegimos una clave ya establecida
```

---

## 6️⃣ Paso 6: Configuración de Red

### 🌐 ¿Quién puede acceder?

```
Configuración de red:
    🌍 Define el acceso a tu instancia
    🚪 Qué tráfico permites
    🔒 Qué tráfico bloqueas
```

### 🎯 Para un servidor web

```
Lo que necesitamos:
    ✅ Permitir tráfico HTTP desde internet
    
¿Por qué?
    🌐 Es un servidor WEB
    👥 La gente necesita acceder
    📡 Desde cualquier lugar de internet
    
Configuración:
    HTTP → ABIERTO al mundo 🌍
```

### 💡 Más detalles después

> **Nos divertiremos mucho revisando estos datos un poco más adelante**, pero por ahora, basta con permitir HTTP desde internet. 🎯

---

## 7️⃣ Paso 7: Opciones de Almacenamiento

### 💾 ¿Cuánto espacio en disco?

```
Almacenamiento para la instancia:
    📦 Espacio para archivos
    💽 Sistema operativo
    📄 Tu contenido web
```

### 🎯 Para esta demo

```
Configuración:
    💾 8 GB de espacio en disco
    📦 Volumen gp3 de EBS
    
EBS = Elastic Block Store
    💽 Almacenamiento persistente
    🔄 Se puede modificar
    ⚡ Rápido y confiable
    
8 GB:
    ✅ Suficiente espacio para el servicio web
    ✅ Sistema operativo
    ✅ Tus archivos web básicos
```

---

## 8️⃣ Paso 8: Datos de Usuario (¡El Truco Secreto!)

### 🎩 La magia de la automatización

```
Problema:
    La AMI de Amazon Linux es genérica
    NO tiene servidor web activado al lanzar
    
Solución:
    🪄 ¡Datos de usuario!
```

### 🤔 ¿Qué son los Datos de Usuario?

```
Datos de usuario:
    📜 Script que se ejecuta AL INICIO
    🤖 Automatiza configuración inicial
    ⚡ Se ejecuta una sola vez
    
    = "Instrucciones del primer día"
```

### 🎯 Dónde encontrarlo

```
En la consola:
    Detalles avanzados
        ↓
    Sección "Datos de usuario"
        ↓
    Pegar tu script aquí 📝
```

### 💻 El script para servidor web

```bash
#!/bin/bash
# Script para instalar y activar Nginx

# Instalar Nginx
[comandos de instalación]

# Activar Nginx
[comandos para iniciar servicio]

# Configurar para que inicie automáticamente
[comandos de autostart]
```

**Este script:**
- ✅ Instala el servidor web Nginx
- ✅ Lo activa automáticamente
- ✅ Lo configura para enviar contenido a internet

---

## 9️⃣ Paso 9: ¡LANZAR!

### 🚀 El momento de la verdad

```
Todo configurado:
    ✅ Nombre
    ✅ AMI (Amazon Linux)
    ✅ Tipo (t2.micro)
    ✅ Par de claves
    ✅ Red (HTTP permitido)
    ✅ Almacenamiento (8 GB)
    ✅ Datos de usuario (script Nginx)
    
Ahora:
    🖱️ Click en "Lanzar instancia"
    ⏰ Esperar unos segundos...
    ✅ ¡INSTANCIA CREADA!
```

### 🎯 Después del lanzamiento

```
La consola te muestra:
    📊 Estado de la instancia
    🔍 Detalles técnicos
    🌐 Dirección IP pública
    ⚙️ Configuración completa
```

---

## 🎉 Paso 10: ¡Probar Tu Servidor Web!

### 🌐 Ver tu creación en acción

```
PASO 1: Copiar la IP pública
    📋 En la consola de EC2
    🔍 Buscar "Dirección IP pública"
    📝 Ejemplo: 54.123.456.789
    
PASO 2: Abrir navegador
    🌐 Chrome, Firefox, Safari...
    
PASO 3: Pegar la IP en la barra de dirección
    http://54.123.456.789
    
PASO 4: ¡Enter!
    ⏰ Esperar 1 segundo...
    ✨ ¡Ahí está!
```

### 🎊 ¡LO LOGRASTE!

```
        🎉 ¡ÉXITO! 🎉
            
    Tu propia instancia de EC2
    ejecutando un servidor web básico
    ¡Accesible desde CUALQUIER LUGAR!
    
    🌍 → 🌐 → 🖥️ → ✅
```

---

## 📊 Resumen Visual del Proceso Completo

```
┌─────────────────────────────────────────────┐
│     🚀 PROCESO DE LANZAMIENTO EC2          │
└─────────────────────────────────────────────┘

1. Consola EC2 🌐
   └→ "Lanzar instancia"
        ↓
2. Nombre 📛
   └→ "mi-servidor-web"
        ↓
3. AMI 🖼️
   └→ Amazon Linux
        ↓
4. Tipo 💻
   └→ t2.micro (1 vCPU, 1 GB RAM)
        ↓
5. Par de claves 🔐
   └→ Seleccionar o crear
        ↓
6. Red 🌐
   └→ Permitir HTTP desde internet
        ↓
7. Almacenamiento 💾
   └→ 8 GB gp3 EBS
        ↓
8. Datos de usuario 📜
   └→ Script para instalar Nginx
        ↓
9. Lanzar 🚀
   └→ Click en botón
        ↓
10. ¡Funciona! ✅
    └→ http://TU-IP-PUBLICA
```

---

## 🎨 Las AMI: Plantillas Mágicas

### 🖼️ ¿Por qué son importantes?

```
AMI (Amazon Machine Image):
    
    📦 Imagen de máquina virtual prediseñada
    🧩 Componentes básicos incluidos
    ⚡ Lista para iniciar instancia
    
    = "Fotocopia perfecta de un servidor"
```

### 🎯 Beneficios de las AMI

```
✅ Mantiene COHERENCIA
    → Todas las instancias iguales
    
✅ Aumenta EFICIENCIA
    → No configurar cada vez desde cero
    
✅ Facilita ESCALADO
    → Crear 100 instancias idénticas fácil
    
✅ Ahorra TIEMPO
    → De horas a minutos
```

### 🔄 AMI en acción

```
Escenario: Necesitas 10 servidores idénticos

SIN AMI:
    ⏰ Configurar servidor 1 (2 horas)
    ⏰ Configurar servidor 2 (2 horas)
    ⏰ ... (repite 10 veces)
    ❌ Posibles diferencias entre servidores
    😱 TOTAL: 20 horas
    
CON AMI:
    🖼️ Creas servidor perfecto
    📸 Haces AMI de ese servidor
    🚀 Lanzas 10 instancias de esa AMI
    ✅ Todas IDÉNTICAS
    ⚡ TOTAL: 10 minutos
```

---

## 💡 Configuraciones Clave que Aprendiste

### 📋 Checklist de configuración

```diff
+ Nombre: Identifica tu instancia
+ AMI: La plantilla base de tu servidor
+ Tipo de instancia: La potencia (CPU/RAM)
+ Par de claves: Tu llave de acceso SSH
+ Configuración de red: Quién puede acceder
+ Almacenamiento: Cuánto espacio en disco
+ Datos de usuario: Scripts de automatización
```

### 🎯 Cada configuración tiene su propósito

| Configuración | ¿Qué Define? | Ejemplo |
|---------------|-------------|---------|
| **Nombre** | Identificación | "mi-servidor-web" |
| **AMI** | Sistema operativo y apps | Amazon Linux |
| **Tipo** | Recursos (CPU/RAM) | t2.micro (1 vCPU, 1 GB) |
| **Claves** | Acceso seguro | mi-clave.pem |
| **Red** | Tráfico permitido | HTTP desde internet |
| **Almacenamiento** | Espacio en disco | 8 GB gp3 |
| **Datos de usuario** | Automatización inicial | Script Nginx |

---

## 🎮 ¿Qué Acabas de Crear?

### 🖥️ Tu servidor web explicado

```
Tu instancia EC2:
    
    🌍 Accesible desde INTERNET
        ↓
    🌐 Servidor web Nginx funcionando
        ↓
    🐧 Amazon Linux como sistema operativo
        ↓
    💻 1 vCPU y 1 GB RAM
        ↓
    💾 8 GB de almacenamiento
        ↓
    ☁️ Corriendo en AWS
        ↓
    🔒 Seguro con tu par de claves
```

### 🎯 Capacidades de tu servidor

```
✅ Responde a peticiones HTTP
✅ Puede servir páginas web
✅ Está en la nube de AWS
✅ Escalable (puedes hacer más grande)
✅ Lo controlas tú completamente
```

---

## 🚀 ¿Y Ahora Qué?

### 🎯 Próximos pasos

```
NIVEL 1 (Completado ✅):
    ✅ Lanzaste tu primera instancia
    ✅ Tienes un servidor web básico
    ✅ Entiendes las configuraciones clave
    
NIVEL 2 (A continuación):
    🔍 Explorar más configuraciones de red
    📊 Entender EBS en detalle
    🔐 Profundizar en seguridad
    🎨 Personalizar tu AMI
    
NIVEL 3 (Más adelante):
    🤖 Automatización completa
    📈 Auto Scaling
    🌍 Despliegue multi-región
    🏆 ¡Arquitecto AWS!
```

---

## 💭 Reflexión: Lo Que Aprendiste

### ✨ Antes vs Ahora

```
❌ ANTES:
    "EC2 suena complicado"
    "No sé cómo crear un servidor"
    "¿AMI? ¿Qué es eso?"
    
✅ AHORA:
    "Acabo de crear un servidor web"
    "Sé qué es una AMI y para qué sirve"
    "Entiendo las configuraciones clave"
    "¡Puedo hacerlo de nuevo!"
```

---

## 🎯 Puntos Clave para Recordar

```diff
+ Lanzar una instancia EC2 es FÁCIL
+ La consola te guía paso a paso
+ AMI = Plantilla de tu servidor
+ t2.micro = Gratis y perfecto para aprender
+ Datos de usuario = Automatización inicial
+ Par de claves = Tu llave de acceso
+ En minutos tienes un servidor funcionando
+ AMI mantiene coherencia y eficiencia
+ Puedes escalar fácilmente con AMI
```

---

## 🎓 Configuración Resumida

### 📋 La receta completa

```
TU PRIMER SERVIDOR WEB EN EC2:

Ingredientes:
    📛 Nombre: mi-servidor-web
    🖼️ AMI: Amazon Linux
    💻 Tipo: t2.micro (FREE TIER)
    🔐 Claves: Tu par de claves SSH
    🌐 Red: HTTP permitido
    💾 Disco: 8 GB gp3
    📜 Script: Instalar Nginx
    
Tiempo de preparación: ⏰ 5 minutos
Dificultad: 🌟 Fácil
Resultado: ✅ Servidor web funcionando

¡A disfrutar! 🎉
```

---

## 🎊 ¡Enhorabuena!

### 🏆 Lo que lograste hoy

```
✨ Completaste tu primera instancia EC2
✨ Creaste un servidor web desde cero
✨ Aprendiste sobre AMI
✨ Entiendes configuraciones clave
✨ Viste el proceso completo en acción

= ¡ERES UN CREADOR DE SERVIDORES! 🚀
```

---

## 💡 Consejos Finales

### 🎯 Para tu siguiente instancia

```
1️⃣ Experimenta con diferentes AMI
2️⃣ Prueba otros tipos de instancia
3️⃣ Juega con scripts de datos de usuario
4️⃣ Explora configuraciones de red
5️⃣ Crea tu propia AMI personalizada

Recuerda:
    ⚠️ Esto es lo BÁSICO
    📚 Veremos más detalles adelante
    🎓 Sigue aprendiendo
    🚀 No te pierdas nada
```

---

<div align="center">

## 🎯 ¡Misión Cumplida!

### Has lanzado tu primera instancia EC2 🚀

**De cero a servidor web en minutos** ⚡

---

### 💭 Recuerda

*"Esto es lo básico sobre configurar instancias de EC2.  
Veremos más detalles sobre los matices adelante en el curso."* 🎓

---

### 🌟 ¡Sigue Practicando!

**Cada instancia que lances te hace más experto** 🏆

---

### 🚀 Tu Viaje en AWS Continúa

**El próximo paso: profundizar en cada configuración** ✨

</div>

---

## 📚 Glosario Rápido

| Término | Significado |
|---------|-------------|
| **AMI** | Plantilla prediseñada de máquina virtual |
| **t2.micro** | Tipo de instancia pequeña (1 vCPU, 1 GB RAM) |
| **Par de claves** | Clave pública + privada para acceso SSH |
| **EBS** | Elastic Block Store - Almacenamiento persistente |
| **gp3** | Tipo de volumen EBS de propósito general |
| **Datos de usuario** | Script que se ejecuta al iniciar la instancia |
| **HTTP** | Protocolo de transferencia de hipertexto |
| **Nginx** | Servidor web de alto rendimiento |
| **IP pública** | Dirección de internet de tu instancia |
| **vCPU** | CPU virtual (núcleo de procesamiento virtual) |
