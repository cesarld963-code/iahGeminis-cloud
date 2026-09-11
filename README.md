# iahGeminis Cloud

> Plataforma inteligente de integración con IA basada en Google Cloud Platform y Google AI Studio.

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Last Updated](https://img.shields.io/badge/Last%20Updated-2026--09-brightgreen)]()

## 📋 Tabla de Contenidos

- [Descripción](#descripción)
- [Características](#características)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Uso](#uso)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Configuración](#configuración)
- [Seguridad](#seguridad)
- [Licencia](#licencia)
- [Contacto](#contacto)

## 📝 Descripción

iahGeminis es una plataforma de código abierto que implementa un sistema de toma de decisiones basado en IA, donde toda formulación de idea genera respuestas coherentes que promueven el bien común, flexibilidad y tolerancia en la resolución de problemas.

**Filosofía del Proyecto:**
> Toda formulación de idea debe crear una respuesta a la toma de cada decisión o bien opción, que como resultado sea en todo momento o instante de bien común, para lograr flexibilidad y tolerancia, donde pudiese haber llegado a tener un quebranto, siendo la base de todo sistema código o pensamiento y tener un resultado fiable y de confianza total.

## ✨ Características

- 🤖 Integración con Google Gemini Pro/Flash v1
- ☁️ Infraestructura en Google Cloud Platform
- 🔐 Seguridad de nivel empresarial (TLS, encriptación)
- 🌍 Soporte multiidioma
- 📊 APIs RESTful documentadas
- 🧪 Suite de pruebas completa
- 🚀 Despliegue en localhost y entornos cloud

## 🔧 Requisitos

- Python 3.9+
- Google Cloud SDK
- Credenciales de Google Cloud (API key o service account)
- pip (gestor de paquetes de Python)

## 📦 Instalación

```bash
# Clonar el repositorio
git clone https://github.com/cesarld963-code/iahGeminis-cloud.git
cd iahGeminis-cloud

# Crear entorno virtual
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# Instalar dependencias
pip install -r requirements.txt

# Configurar variables de entorno
cp .env.example .env
# Editar .env con tus credenciales de Google Cloud
```

## 🚀 Uso

### Inicio rápido

```python
from iogeminis import GeminiAgent

# Inicializar el agente
agent = GeminiAgent(api_key="tu-api-key")

# Hacer una consulta
respuesta = agent.consultar("¿Cómo puedo optimizar este proceso?")
print(respuesta)
```

### Ejecución local (desarrollo)

```bash
# Servidor de desarrollo
python app.py

# Acceder a: http://localhost:8000
```

## 📂 Estructura del Proyecto

```
iahGeminis-cloud/
├── .github/
│   ├── workflows/        # GitHub Actions CI/CD
│   ├── ISSUE_TEMPLATE/   # Plantillas de issues
│   └── PULL_REQUEST_TEMPLATE/
├── src/
│   ├── iogeminis/       # Código principal del paquete
│   ├── app.py           # Aplicación principal
│   └── config.py        # Configuración
├── tests/               # Suite de pruebas
├── docs/                # Documentación
├── requirements.txt     # Dependencias de Python
├── .env.example         # Variables de entorno (ejemplo)
├── LICENSE              # Licencia Apache 2.0
└── README.md            # Este archivo
```

## ⚙️ Configuración

### Variables de Entorno

```env
# Google Cloud
GOOGLE_API_KEY=your-api-key-here
GOOGLE_PROJECT_ID=your-project-id
GOOGLE_APPLICATION_CREDENTIALS=/path/to/credentials.json

# Aplicación
ENVIRONMENT=development
DEBUG=True
LOG_LEVEL=INFO
```

### Configuración de Seguridad (localhost 127.0.0.1)

El despliegue en 127.0.0.1 (loopback) está diseñado para desarrollo seguro:

- ✅ Aislamiento de tráfico: sin exposición a redes públicas
- ✅ Cifrado TLS: todas las conexiones a Google APIs están encriptadas
- ✅ Cumplimiento SDLC: sigue estándares de desarrollo seguro
- ✅ Sin puertos públicos: requiere proxy inverso para producción

## 🔒 Seguridad

### Reportes de Seguridad

Para reportes de vulnerabilidades de seguridad:

📧 **Contacto**: Julio César Argüello Pérez
📨 **Correo de seguridad**: [security@iogeminis.app]
⚠️ **NO reportar públicamente en issues**

### Política de Seguridad

- Auditorías periódicas de código
- Uso de bibliotecas confiables (Apache Software Foundation, jsoup MIT)
- Validación de entrada en todos los endpoints
- Secrets management seguro

## 📄 Licencia

Este proyecto se distribuye bajo la **Apache License 2.0**.

```
Copyright © 2026 iahGeminis. Todos los derechos reservados.
Prohibida la reproducción total o parcial sin la debida atribución.
```

Ver archivo [LICENSE](LICENSE) para detalles completos.

### Dependencias de Terceros

- Apache Software Foundation libraries (Apache 2.0)
- jsoup (MIT License)
- Google Cloud Python Client (Apache 2.0)

Consulta `requirements.txt` para la lista completa.

## 📞 Contacto y Soporte

| Tipo | Contacto |
|------|----------|
| 👨‍💻 **Desarrollador** | Julio César Argüello Pérez |
| 🔐 **Seguridad** | Reportes confidenciales |
| 💬 **Issues** | [GitHub Issues](https://github.com/cesarld963-code/iahGeminis-cloud/issues) |
| 📖 **Documentación** | [Wiki del Proyecto](https://github.com/cesarld963-code/iahGeminis-cloud/wiki) |

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Fork el repositorio
2. Crea una rama (`git checkout -b feature/nueva-caracteristica`)
3. Realiza tus cambios con commits descriptivos
4. Envía un Pull Request
5. Espera revisión y feedback

## 📚 Recursos Adicionales

- [Documentación Completa](docs/)
- [API Reference](docs/api/)
- [Guía de Contribución](CONTRIBUTING.md)
- [Changelog](CHANGELOG.md)

---

**Última actualización**: 2026-09-11 | Versión: 0.1.0
