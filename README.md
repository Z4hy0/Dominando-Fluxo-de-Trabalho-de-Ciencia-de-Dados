# 📊 Miniguia de Estudos: Dominando o Fluxo de Trabalho de Ciência de Dados e Estruturas de Modelagem

![Status do Projeto](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)
![Tecnologia](https://img.shields.io/badge/Ferramenta-NotebookLM-blue)
![Plataforma](https://img.shields.io/badge/DIO-Projeto--Pr%C3%A1tico-orange)

## 🎯 Contexto e Objetivos

Este repositório documenta a construção de um caderno temático no **NotebookLM** como parte do Desafio de Projeto da **DIO (Digital Innovation One)**, aplicando o conceito de aprendizagem ativa potencializada por IA.

O tema central investigado foi **Fluxos de Trabalho Modernos em Ciência de Dados, Diretrizes Arquiteturais e Boas Práticas em Python**.

### Objetivos de Aprendizagem:
* Compreender a estruturação profissional de diretórios para projetos analíticos escaláveis (`/data/raw`, `/data/processed`, `/src`, etc.).
* Explorar novas ferramentas do ecossistema moderno de dados, como **DuckDB** para consultas analíticas locais, **Positron IDE**, **Pandera** para validação de dados e **Quarto** para relatórios reprodutíveis.
* Utilizar a Engenharia de Prompts no **NotebookLM** para sintetizar referências de artigos técnicos, documentações e pesquisas de mercado (como a Stack Overflow Developer Survey).

---

## 📂 Curadoria de Fontes

O caderno foi alimentado com **18 fontes abertas e materiais técnicos de alta relevância**, dos quais se destacam:

1. **Python para Análise de Dados: Diretrizes Arquiteturais, Engenharia de Software e Práticas de Validação Corporativa**
   * *Descrição:* Guia sobre isolamento de dados brutos, padronização do diretório `/src` e pipelines de I/O.
2. **[Data Modeling: Best Practices for Scalable Python Workflows - Anaconda](https://www.anaconda.com/blog/data-modeling)**
   * *Descrição:* Boas práticas para modelagem de dados e pipelines escaláveis em ambiente Python.
3. **[Why Data Analysts Are Choosing DuckDB for Modern Analytics - DataMites](https://datamites.com/blog/why-data-analysts-are-choosing-duckdb-for-modern-analytics/)**
   * *Descrição:* Análise da ascensão do DuckDB no processamento local analítico sem dependência imediata de clusters em nuvem.
4. **[Positron IDE: Welcome Guide](https://positron.posit.co/welcome.html)**
   * *Descrição:* Documentação da nova IDE focada em Ciência de Dados criada pela Posit.
5. **[A Step-by-Step Guide to the Data Science Workflow - DASCA](https://www.dasca.org/world-of-data-science/article/a-step-by-step-guide-to-the-data-science-workflow)**
   * *Descrição:* Guia passo a passo sobre o ciclo de vida e governança no fluxo de trabalho de Data Science.

---

## 🛠️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

### 🧪 Testes de Prompts e Evolução

* **Tentativa 1 (Prompt Genérico):**
  > *"Como organizar um projeto de ciência de dados em Python?"*
  * **Resultado:** Resposta genérica sobre criar pastas, sem detalhar padrões de imutabilidade ou regras de acesso.
  
* **Tentativa 2 (Prompt Estruturado com Padrões de Arquitetura):**
  > *"Com base nas fontes fornecidas sobre arquitetura e engenharia de software em Python, liste a estrutura ideal de diretórios para um projeto analítico, explicando a regra de imutabilidade da pasta `/data/raw` e a função do diretório `/src`."*
  * **Resultado:** Resposta precisa e técnica, extraindo diretamente as diretrizes de separação de código produtivo e proteção contra alteração dos dados originais.

### ⚠️ Dificuldades Encontradas ("Cicatrizes") e Soluções:
* **Ambiguidade entre Análise Exploratória e Código de Produção:** Ao perguntar sobre Jupyter Notebooks, a IA tendeu a tratar notebooks como local ideal para todo o código.
* **Solução:** Ajustei o prompt para exigir a separação clara entre prototipagem (`/notebooks`) e módulos reutilizáveis de produção (`/src`).

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado do Tema
* **Arquitetura de Projetos:** Dados brutos (`/data/raw`) devem ser estritamente imutáveis. Toda lógica transformadora deve residir em scripts na pasta `/src`.
* **Ecossistema Moderno:** O uso de bancos colunares em memória como **DuckDB** reduz a necessidade de infraestrutura pesada para volumes médios de dados.
* **Documentação Reprodutível:** Ferramentas como **Quarto** unificam código executável e texto Markdown em relatórios profissionais em PDF, HTML ou Word.

### 📚 2. Glossário de Conceitos-Chave
| Termo | Definição Rápida |
| :--- | :--- |
| **Imutabilidade de Raw Data** | Princípio de que os dados originais brutos nunca devem ser alterados para garantir reprodutibilidade. |
| **DuckDB** | SGDB colunar em memória altamente otimizado para consultas OLAP e análise de dados local. |
| **Quarto** | Sistema de publicação técnica e científica que gera relatórios dinâmicos a partir de arquivos `.qmd`. |
| **Positron** | IDE voltada para Ciência de Dados criada sobre Code OSS pela Posit (criadores do RStudio). |

### 🔁 3. Prompts Reutilizáveis para Revisão Futura

1. **Prompt para Mapeamento de Arquitetura:**
   > *"Com base nas fontes anexadas, resuma a finalidade operacional e as regras de manipulação para as pastas `/data/raw`, `/data/processed` e `/src` em um pipeline analítico."*

2. **Prompt para Comparativo de Ferramentas:**
   > *"Extraia das fontes as principais razões técnicas pelas quais desenvolvedores e analistas estão adotando o DuckDB e a IDE Positron para fluxos de dados em Python."*

---

## 🚀 Como Consultar
1. Acesse o Caderno Temático no NotebookLM: [📊 Dominando o Fluxo de Trabalho de Ciência de Dados e as Estruturas de Modelagem Estruturada](https://notebooklm.google.com/notebook/af22a3c6-79c9-4b7c-8812-dcec434691dd)
2. Utilize os prompts sugeridos acima para continuar explorando o material.

---
*Projeto desenvolvido como parte do Desafio de Projeto na [DIO (Digital Innovation One)](https://www.dio.me/).*
