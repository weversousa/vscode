# VSCode

Passo a passo para abrir o arquivo de configuração:
* Manage (Gerir)
  * Settings (Configurações)
    * Open Settings JSON (Abra Configurações)

## Python

Extensões:
* Python da Microsoft
* Pylance da Microsoft
* isort da Microsoft

Configuração:
~~~json
{
  // Vai sinalizar os erros de escrita.
  "python.linting.flake8Enabled": true,

  // Vai sinalizar os erros de tipagem.
  "python.linting.mypyEnabled": true
}
~~~

~~~bash
# Uma única vez em uma máquina (Windows).
~$ Set-ExecutionPolicy Unrestricted -Force

# Uma única vez em uma máquina.
~$ pip install virtualenv

# Criar um ambiente virtual para cada projeto.
~$ python -m venv .venv/

# Ativar o ambiente virtual.
~$ source .venv/bin/activate

# Instalar bibliotecas que facilitam o desenvolvimento em Python.
~$ pip install --upgrade pip flake8 autopep8 mypy
~~~

## Code Runner

Extensões:
* Code Runner de Jun Han

Configuração:
~~~json
{
  "code-runner.executorMap": {
    // Padrão "python -U"
    "python": "clear; ./.venv/bin/python"
  }
}
~~~
