# Aprendizaje Profundo - Especialización en Inteligencia Artificial (CEIA - FIUBA)

Este repositorio contiene los trabajos prácticos desarrollados durante la cursada de la materia Aprendizaje Profundo en la Facultad de Ingeniería de la Universidad de Buenos Aires (FIUBA).

## 📖 Contenido del Repositorio

| Trabajo | Tema | Carpeta |
|---------|------|---------|
| TP 1 | _A definir_ | [`TP1/`](TP1/) |
| TP 2 | _A definir_ | [`TP2/`](TP2/) |
| TP 3 | _A definir_ | [`TP3/`](TP3/) |

## 🛠️ Tecnologías Utilizadas

- Python 3.11
- PyTorch (con soporte CUDA 13.0)
- NumPy, Pandas, SciPy, Scikit-Learn, XGBoost
- Matplotlib, Seaborn
- Jupyter Notebooks
- [uv](https://docs.astral.sh/uv/) para la gestión del entorno

## ⚙️ Configuración del Entorno

Requisitos: tener [uv](https://docs.astral.sh/uv/getting-started/installation/) instalado.

```bash
git clone https://github.com/NicoLastra12/CEIA-Aprendizaje_profundo.git
cd CEIA-Aprendizaje_profundo
uv sync
```

`uv sync` crea el entorno virtual (`.venv`) con Python 3.11 e instala las versiones exactas definidas en `uv.lock`.

Para usar el entorno desde Jupyter, registrar el kernel:

```bash
uv run python -m ipykernel install --user --name ceia_aprendizaje_profundo --display-name "CEIA - Aprendizaje profundo"
```

Luego, seleccionar el kernel **Python 3.11 (Aprendizaje Profundo)** desde Jupyter o VS Code.

### GPU

PyTorch se instala desde el índice de CUDA 13.0 (`cu130`), por lo que requiere una GPU NVIDIA con un driver que soporte CUDA 13.0 o superior (verificable con `nvidia-smi`). Para comprobar que la GPU está disponible:

```bash
uv run python -c "import torch; print(torch.__version__, torch.cuda.is_available())"
```

## 📚 Material de la Materia

El material de clases oficial se encuentra en el [repositorio de la cátedra](https://github.com/FIUBA-Posgrado-Inteligencia-Artificial/aprendizaje_profundo).