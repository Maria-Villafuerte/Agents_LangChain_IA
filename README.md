# Agents_LangChain_IA
Esta aplicación implementa un agente inteligente utilizando LangChain y OpenAI GPT-4 que puede ejecutar código Python y analizar archivos CSV. El agente puede responder preguntas mediante la ejecución de código Python y realizar análisis de datos sobre archivos CSV.

## Características
- Ejecución de código Python en tiempo real
- Análisis de archivos CSV
- Integración con GPT-4
- Sistema de herramientas extensible
- Manejo de variables de entorno para configuraciones seguras

## Requisitos Previos
- Python 3.8 o superior
- Clave API de OpenAI
- Instalación de paquetes necesarios (ver requirements.txt)

## Instalación

1. Clonar el repositorio:
```bash
git clone https://github.com/Maria-Villafuerte/Agents_LangChain_IA
cd Agents_LangChain_IA
python main.py

```

2. Crear un entorno virtual:
```bash
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
```

3. Instalar las dependencias:
```bash
pip install -r .\requirements.txt
```

4. Configurar las variables de entorno:
   - Crear un archivo `.env` en el directorio raíz
   - Agregar tu clave API de OpenAI:
```
OPENAI_API_KEY=tu-clave-api
```

## Estructura del Proyecto
```
.
├── .env                    # Variables de entorno
├── main.py                 # Archivo principal
└── episode_info.csv        # Archivo CSV de ejemplo
```



### Ejemplos de Uso

1. Agente Python:
```bash
agent_executor.invoke(
    input={
        "input": "generate and save in current working directory 2 QR codes"
    }
)
```

2. Agente CSV:
```bash
csv_agent.invoke(
    input={
        "input": "how many columns are there in the file episode_info.csv?"
    }
)
```
