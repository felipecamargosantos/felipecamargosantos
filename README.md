# Olá, sou o Felipe Camargo1 👋

Engenheiro focado na interseção entre **Engenharia de Dados**, **MLOps Produtivo** e **Sistemas Distribuídos**. Desenvolvo esteiras de dados resilientes, APIs de Machine Learning orientadas a métricas de negócio e arquiteturas em tempo real.

---

### 🚀 Projetos em Destaque

| Projeto | Problema & Solução de Engenharia | Stack Tecnológica |
|---|---|---|
| [**etl-data-warehouse**](https://github.com/SEU_USUARIO/etl-data-warehouse) | Ingestão resiliente de séries financeiras do Banco Central com carga incremental via `MERGE` e **Hash Diff (SHA-256)** no SQL Server, reduzindo I/O e validando regimes de volatilidade com **Teste t e ANOVA (SciPy)**. | `Python 3.11` `SQL Server` `Docker` `Pandas` `SQLAlchemy` `SciPy` |
| [**churn-mlops-service**](https://github.com/SEU_USUARIO/churn-mlops-service) | Microsserviço de inferência de Churn com pipeline serializado único (`ColumnTransformer` + `XGBoost`). Substituição do corte padrão de 50% por **otimização de threshold via matriz de custo financeiro** e explicabilidade em tempo real com **SHAP**. | `FastAPI` `XGBoost` `MLOps` `Docker` `SHAP` `Pydantic` `Pytest` |
| [**market-price-comparator**](https://github.com/SEU_USUARIO/SEU_REPOSITORIO_MERCADO) | Arquitetura distribuída de inteligência competitiva de preços: spiders concorrentes em **Node.js**, motor de normalização e deduplicação de catálogos em **Java**, e alertas em tempo real via **Supabase (WebSockets)**. | `Java` `Node.js` `Supabase` `PostgreSQL` `WebSockets` `Web Scraping` |

---

### 🛠️ Competências & Ferramentas
┌───────────────────────────────┬─────────────────────────────────────────────────────────┐
│ Domínio                       │ Tecnologias & Conceitos Práticos                        │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Engenharia de Dados & DW      │ Python, SQL (T-SQL, PostgreSQL), Carga Incremental,     │
│                               │ Hash Diff (SHA-256), Modelagem Dimensional, Pandas      │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Machine Learning & MLOps      │ XGBoost, Scikit-Learn, Serialização (Joblib), SHAP,     │
│                               │ Otimização de Threshold Financeiro, Prevenção Leakage   │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Backend & APIs                │ FastAPI, Node.js, Java, Pydantic, RESTful APIs,         │
│                               │ WebSockets (Realtime), Pytest, TestClient               │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Banco de Dados & Infra        │ SQL Server, PostgreSQL, Supabase, Docker, Git/GitHub    │
└───────────────────────────────┴─────────────────────────────────────────────────────────┘

---

### 📈 Princípios de Arquitetura que Aplico no Código

- **Prevenção de Training-Serving Skew:** O pré-processamento viaja encapsulado dentro do pipeline serializado do modelo, sem regras manuais soltas na API.
- **Idempotência e Performance de Escrita:** Cargas em banco comparam assinaturas de hash para evitar leituras e gravações desnecessárias (`TRUNCATE + INSERT`).
- **Validação Estrita de Contrato:** Uso de tipagem estrita com Pydantic para rejeitar requisições malformadas na borda antes de onerar os motores de banco ou ML.

---

### 📬 Onde me encontrar

[![LinkedIn](https://www.linkedin.com/in/felipecamargosantos/)
