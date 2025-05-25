# 📊 Linguagens de Programação em Repositórios do GitHub

Este projeto automatiza a coleta, análise e publicação de dados sobre as linguagens de programação mais utilizadas por empresas como **Amazon**, **Netflix** e **Spotify** em seus repositórios públicos no GitHub.

---

## ✨ Funcionalidades

✅ Coleta os repositórios públicos de um usuário ou organização no GitHub  
✅ Extrai o nome dos repositórios e suas linguagens principais  
✅ Cria um DataFrame com os dados obtidos  
✅ Salva os dados em arquivos `.csv`  
✅ Cria um novo repositório no GitHub do usuário autenticado  
✅ Faz upload automático dos arquivos `.csv` para esse novo repositório

---

## 🧠 Tecnologias Utilizadas

- Python 3
- [GitHub API REST](https://docs.github.com/pt/rest)
- `requests`
- `pandas`
- `python-dotenv`
- `base64` (para envio de arquivos)

---

## 📁 Estrutura do Projeto

```
├── dados/
│   ├── linguagens_amzn.csv
│   ├── linguagens_netflix.csv
│   └── linguagens_spotify.csv
├── coleta_dados.py
├── publica_dados.py
├── .env
└── README.md
```

---

## ⚙️ Como Executar o Projeto

### 1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

### 2. Instale as dependências:

```bash
pip install -r requirements.txt
```

> Arquivo `requirements.txt` sugerido:
```
requests
pandas
python-dotenv
```

### 3. Configure a variável de ambiente:

Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:

```
GITHUB_TOKEN=seu_token_pessoal
```

> ⚠️ Você pode gerar um [token de acesso pessoal no GitHub aqui](https://github.com/settings/tokens) com permissões para `repo`.

---

### 4. Execute os scripts

#### Coleta de dados:
```bash
python coleta_dados.py
```

#### Criação de repositório e envio dos arquivos:
```bash
python publica_dados.py
```

---

## 📝 Sobre os Dados

Os dados são coletados diretamente dos repositórios públicos das organizações:

- [`amzn`](https://github.com/amzn)
- [`netflix`](https://github.com/netflix)
- [`spotify`](https://github.com/spotify)

O resultado é um conjunto de arquivos `.csv` contendo os nomes dos repositórios e suas linguagens principais de programação.

---

## 📬 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias.

---

## 🧑‍💻 Autor

- **Raphael Lima** — [@PhaelLima-j](https://github.com/PhaelLima-j)
