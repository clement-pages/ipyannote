# ipyannote

## Installation

```sh
pip install ipyannote
```

## Development installation

Clone the repo

```sh
git clone https://github.com/hbredin/ipyannote
cd ipyannote
```

Create a virtual environment and and install ipyannote in *editable* mode with the
optional development dependencies:

```sh
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
```

You then need to install the JavaScript dependencies and run the development server.

```sh
npm install
npm run dev
```

Change the `DEV` variable to `True` in `src/ipyannote/__init__.py` so that the widget gets its frontend code from the development server.

Start Jupyter Lab with hot module reloading enabled:

```sh
ANYWIDGET_HMR=1 jupyter lab
```

Open `examples/example.ipynb` in JupyterLab, VS Code, or your favorite editor
to start developing. Changes made in `js/` will be reflected
in the notebook.
