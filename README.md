# PostgreSQL Data Project

Proyecto base para analisis de datos de clientes con PostgreSQL y Python.

## Requisitos

- Python 3.13 o superior
- PostgreSQL en ejecucion

## Instalacion

Opcion recomendada con `uv`:

```bash
uv sync
```

Opcion alternativa con `pip`:

```bash
pip install -e .
```

## Configuracion

1. Copia el archivo de ejemplo:

```bash
cp .env.example .env
```

En PowerShell:

```powershell
Copy-Item .env.example .env
```

2. Ajusta los valores de conexion en `.env`:

- `PGHOST`
- `PGPORT`
- `PGDATABASE`
- `PGUSER`
- `PGPASSWORD`

## Estructura del proyecto

- `main.py`: punto de entrada del proyecto.
- `book.ipynb`: notebook para exploracion y analisis.
- `customer.csv`: dataset de ejemplo.
- `pyproject.toml`: configuracion del proyecto y dependencias.
- `.env.example`: plantilla de variables de entorno para PostgreSQL.

## Uso

Ejecutar script principal:

```bash
python main.py
```

Abrir el notebook:

```bash
jupyter notebook book.ipynb
```

## Dependencias principales

- `jupyter`
- `matplotlib`
- `pandas`
- `python-dotenv`
- `psycopg2-binary`
- `seaborn`
- `sqlalchemy`
