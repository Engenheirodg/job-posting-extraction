# 🧠 Projeto de Extração de Vagas - ATS Brasileiros

## 📌 Sobre

Este projeto tem como foco a extração de dados de **vagas de emprego** divulgadas nas **quatro principais plataformas de ATS** (Applicant Tracking System ou Sistema de Rastreamento de Candidatos) do Brasil:

- [Gupy](https://www.gupy.io/)
- [Sólides](https://www.solides.com.br/)
- [Vagas.com.br](https://www.vagas.com.br/)
- [Infojobs](https://www.infojobs.com.br/)

O projeto foi desenvolvido em **Python**, utilizando **crawlers** para coletar **dados públicos** disponibilizados pelas plataformas, respeitando as diretrizes dos arquivos `robots.txt` de cada site (que restringem apenas URLs relacionadas a candidaturas, usuários e área logada das empresas).

---

## 🧰 Tecnologias Utilizadas

- **Linguagem:** Python
- **IDE:** Visual Studio Code
- **Principais bibliotecas:**
  - `selenium`
  - `BeautifulSoup`
  - `pandas`
  - `numpy`
  - `requests`
  - `os`
  - `time`

---

## 🎯 Objetivos

### 👤 Pessoal
Disponibilizar uma página de consulta pública com **as vagas mais recentes** das 4 plataformas, contendo:
- Nome da plataforma
- Nome da vaga
- Local/formato de trabalho
- Link da vaga

### 💼 Profissional
Criar uma base diária de dados para análises de mercado de R&S (Recrutamento e Seleção), com foco em:
- Criação de grupos de cargos
- Medição do tempo de vaga aberta
- Percentual de vagas por grupo de cargo
- Média de tempo em aberto por grupo, região e ATS
- Geração de nuvens de palavras por grupo de cargo
- Identificação de expressões mais utilizadas e requisitos mais comuns
- Análise de tendências sazonais (por localidade, formato de trabalho, etc.)

---

## ⚙️ Metodologia

O código principal é o `main/main.py`, que orquestra a execução dos scripts de cada plataforma.

### 🛠 Estrutura dos scripts por ATS

#### Gupy
- `extracao_gupy.py`: Extrai os dados das vagas
- `textos_gupy.py`: Extrai os textos das descrições
- `dados_gupy.py`: Consolida todos os dados em CSV

#### Infojobs
- `extracao_infojobs.py`
- `textos_infojobs.py`
- `dados_infojobs.py`

#### Vagas.com.br
- `extracao_vagas.py`
- `textos_vagas.py`
- `dados_vagas.py`

#### Sólides
- `extracao_solides.py`
- `textos_solides.py`
- `dados_solides.py`

---

## 🚀 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio

2. Instale as dependências:

   ```bash
   pip install -r requirements.txt

3. Execute o orquestrador:
   ```bash
   python main/main.py

⚠️ É necessário ter o ChromeDriver instalado e compatível com sua versão do navegador, além do navegador Google Chrome.

📄 Licença
Este projeto está sob a licença MIT.

🙌 Agradecimentos
Esse projeto foi idealizado com propósito de estudo e contribuição para o mercado de Recrutamento & Seleção. Feedbacks e colaborações são super bem-vindos!

