# Estrutura do Repositório

Este documento descreve a estrutura e organização dos arquivos neste repositório.

## 📁 Estrutura de Diretórios

```
Stats-In-Codespace/
├── .devcontainer/              # Configuração do GitHub Codespaces
│   ├── devcontainer.json       # Configuração principal do container
│   └── setup.sh                # Script de instalação automática
├── .github/
│   └── workflows/              # GitHub Actions
│       └── validate-devcontainer.yml
├── .gitignore                  # Arquivos ignorados pelo Git
├── README.md                   # Documentação principal
├── QUICKSTART.md              # Guia de início rápido
├── requirements.txt           # Pacotes Python
├── exemplo_estatistica.ipynb  # Notebook exemplo em R
└── exemplo_python.ipynb       # Notebook exemplo em Python
```

## 📄 Descrição dos Arquivos

### Configuração do Ambiente

#### `.devcontainer/devcontainer.json`
Arquivo de configuração principal do GitHub Codespaces que define:
- Imagem base do container (Universal image com Python e R)
- Extensões VS Code instaladas automaticamente
- Configurações do editor
- Comandos de pós-criação
- Portas expostas

#### `.devcontainer/setup.sh`
Script bash executado automaticamente após a criação do Codespace. Instala:
- Jupyter Notebook e JupyterLab
- Pacotes Python (via requirements.txt)
- IRkernel (kernel R para Jupyter)
- Pacotes R para estatística (ggplot2, dplyr, tidyr, etc.)

#### `requirements.txt`
Lista de pacotes Python instalados automaticamente:
- jupyter, jupyterlab, notebook - Ambiente Jupyter
- numpy, pandas - Manipulação de dados
- matplotlib, seaborn, plotly - Visualização
- scipy, scikit-learn, statsmodels - Análise estatística

### Documentação

#### `README.md`
Documentação principal do repositório com:
- Visão geral do projeto
- Instruções de uso (Codespaces e local)
- Como usar Jupyter Notebooks
- Pacotes incluídos
- Recursos adicionais

#### `QUICKSTART.md`
Guia rápido para iniciantes com:
- Passos para criar um Codespace
- Como abrir e executar notebooks
- Criar novos notebooks
- Instalar pacotes adicionais
- Solução de problemas comuns

### Exemplos

#### `exemplo_estatistica.ipynb`
Notebook de exemplo usando R que demonstra:
- Carregamento de bibliotecas (ggplot2, dplyr)
- Criação de dados de exemplo
- Estatísticas descritivas
- Visualização com ggplot2
- Análise por grupos com dplyr

#### `exemplo_python.ipynb`
Notebook de exemplo usando Python que demonstra:
- Importação de bibliotecas (numpy, pandas, matplotlib)
- Criação de dados de exemplo
- Estatísticas descritivas
- Visualização com matplotlib
- Análise por grupos com pandas

### Automação

#### `.github/workflows/validate-devcontainer.yml`
GitHub Action que valida automaticamente:
- Existência do devcontainer.json
- Sintaxe JSON válida
- Existência e permissões do setup.sh
- Existência e conteúdo do requirements.txt

### Controle de Versão

#### `.gitignore`
Exclui do Git:
- Arquivos temporários do Jupyter (.ipynb_checkpoints)
- Cache Python (__pycache__, *.pyc)
- Arquivos do R (.Rhistory, .RData)
- Arquivos de configuração do VS Code (exceto essenciais)
- Arquivos de sistema (macOS, Windows)

## 🔧 Customização

### Adicionar Pacotes Python

Edite `requirements.txt` e adicione o nome do pacote em uma nova linha:
```
novo-pacote==1.0.0
```

### Adicionar Pacotes R

Edite `.devcontainer/setup.sh` e adicione na seção de instalação de pacotes R:
```bash
R -e "install.packages('novo_pacote', repos='https://cloud.r-project.org/')"
```

### Adicionar Extensões VS Code

Edite `.devcontainer/devcontainer.json` na seção `customizations.vscode.extensions`:
```json
"extensions": [
  "ms-python.python",
  "nova.extensao"
]
```

## 🚀 Workflow de Desenvolvimento

1. **Criar Codespace**: GitHub cria o ambiente
2. **Setup Automático**: Script `.devcontainer/setup.sh` executa
3. **Ambiente Pronto**: Jupyter + R + Python configurados
4. **Desenvolvimento**: Criar e executar notebooks
5. **Commit**: Salvar trabalho no Git
6. **Push**: Enviar para o repositório

## 📚 Recursos Técnicos

### Tecnologias Utilizadas

- **GitHub Codespaces**: Ambiente de desenvolvimento na nuvem
- **Dev Containers**: Containerização do ambiente
- **Docker**: Base para containers
- **Jupyter**: Interface de notebooks
- **R**: Linguagem de programação estatística
- **Python**: Linguagem de programação científica
- **VS Code**: Editor de código

### Requisitos

- Conta GitHub (para Codespaces)
- OU Docker instalado (para desenvolvimento local)

## 🔍 Validação

Para validar manualmente a configuração:

```bash
# Validar JSON
python -m json.tool .devcontainer/devcontainer.json

# Verificar permissões
ls -l .devcontainer/setup.sh

# Testar setup (em ambiente com R e Python)
bash .devcontainer/setup.sh
```

## 📊 Métricas

- **Tempo de setup**: ~3-5 minutos (primeira vez)
- **Tamanho do ambiente**: ~2-3 GB
- **Pacotes Python**: 12+
- **Pacotes R**: 10+ (incluindo tidyverse)
