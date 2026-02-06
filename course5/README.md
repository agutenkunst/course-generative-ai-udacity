# Course 5 - HomeMatch Project

## Virtual Environment Setup

This project uses a Python virtual environment located in the `.venv` folder.

### Activating the Virtual Environment

To activate the virtual environment, run:

```bash
source .venv/bin/activate
```

Once activated, your terminal prompt should show `(.venv)` at the beginning.

### Deactivating the Virtual Environment

To deactivate the virtual environment, simply run:

```bash
deactivate
```

### Installing Dependencies

With the virtual environment activated, install the required packages:

```bash
pip install -r requirements.txt
```

### Running the Project

Once the virtual environment is activated and dependencies are installed, you can run the Jupyter notebook:

```bash
jupyter notebook HomeMatch.ipynb
```

## Troubleshooting

### Missing Rust Compiler

If you encounter errors during installation mentioning Rust or `rustc`, you need to install Rust:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Follow the prompts to complete the installation.

### Missing Python Development Headers

If you get errors like `fatal error: Python.h: No such file or directory` during wheel building (especially from `chroma-hnswlib`), install Python development headers:

```bash
sudo apt-get update && sudo apt-get install python3.12-dev
```

Then retry the pip install command.

### General Installation Issues

If pip installation fails, try upgrading pip first:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```
