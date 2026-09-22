# Olá, sou o Felipe Camargo 👋

Desenvolvedor de Software focado na construção de sistemas orientados a dados: esteiras de **Engenharia de Dados (ETL/DW)**, **Machine Learning em Produção (MLOps)** e **APIs Assíncronas de Deep Learning**. 

Combino rigor estatístico e matemático com arquitetura de software limpa, construindo aplicações que vão da ingestão de dados ao deploy de modelos escaláveis.

---

### 🚀 Projetos em Destaque

| Projeto | Problema & Solução de Engenharia | Stack Tecnológica |
|---|---|---|
| [**saas-forecast-platform**](https://github.com/SEU_USUARIO/saas-forecast-platform) | Plataforma SaaS de previsão de demanda com **LSTM (Deep Learning)** desacoplada via **FastAPI (BackgroundTasks / HTTP 202 Accepted)** para evitar timeouts em treinos pesados. Janelamento temporal de 14 dias sem *data leakage*, projeção autoregressiva multi-step e autenticação com **JWT + Bcrypt nativo**. | `Python 3.11` `FastAPI` `TensorFlow/Keras` `SQLAlchemy` `Docker` `Pytest` `Bcrypt` |
| [**churn-mlops-service**](https://github.com/SEU_USUARIO/churn-mlops-service) | Microsserviço de inferência de Churn em tempo real com pipeline serializado único (`ColumnTransformer` + `XGBoost`). Substituição do corte padrão de 50% por **otimização de threshold via matriz de custo financeiro** e interpretabilidade explicável ponta a ponta com **SHAP**. | `FastAPI` `XGBoost` `MLOps` `Docker` `SHAP` `Pydantic` `Pytest` `Scikit-Learn` |
| [**etl-data-warehouse**](https://github.com/SEU_USUARIO/etl-data-warehouse) | Ingestão resiliente de séries financeiras do Banco Central com carga incremental via `MERGE` e **Hash Diff (SHA-256)** no SQL Server, reduzindo I/O e validando regimes de volatilidade temporal com **Teste t e ANOVA (SciPy)**. | `Python 3.11` `SQL Server` `Docker` `Pandas` `SQLAlchemy` `SciPy` `T-SQL` |

---

### 🛠️ Competências & Ferramentas

┌───────────────────────────────┬─────────────────────────────────────────────────────────┐
│ Domínio                       │ Tecnologias & Conceitos Práticos                        │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Engenharia de Software & API  │ FastAPI, Python 3.11, Pydantic, Uvicorn, RESTful APIs,  │
│                               │ Testes Unitários (Pytest), TestClient, Programação OO  │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Machine Learning & MLOps      │ XGBoost, Redes Neurais LSTM (Keras/TensorFlow), SHAP,   │
│                               │ Scikit-Learn, Otimização de Custos, Autoregressão       │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Engenharia de Dados & DW      │ Python, SQL (T-SQL, PostgreSQL, SQLite), SQLAlchemy,     │
│                               │ Carga Incremental, Hash Diff (SHA-256), Pandas, NumPy   │
├───────────────────────────────┼─────────────────────────────────────────────────────────┤
│ Segurança, Banco & Infra      │ JWT (python-jose), Hashing Bcrypt, SQLite, SQL Server,  │
│                               │ Docker, Git / GitHub, Processamento Assíncrono          │
└───────────────────────────────┴─────────────────────────────────────────────────────────┘

---

### 📈 Princípios de Arquitetura que Aplico no Código

- **Processamento Assíncrono Desacoplado (HTTP 202):** Treinamento de redes neurais e processamentos intensivos nunca concorrem no ciclo síncrono da requisição HTTP, garantindo resposta imediata com tracking de status (`job_id`).
- **Prevenção Estrita de Data Leakage:** Em séries temporais e modelos preditivos, normalizações e transformações são ajustadas (`.fit()`) exclusivamente no conjunto histórico de treino, preservando a integridade estatística da validação.
- **Prevenção de Training-Serving Skew:** O pré-processamento viaja encapsulado dentro do pipeline serializado do modelo, sem regras manuais soltas na API.
- **Idempotência e Performance de Escrita:** Cargas em banco comparam assinaturas de hash para evitar leituras e gravações desnecessárias (`TRUNCATE + INSERT`).
- **Segurança e Validação na Borda:** Validação de esquemas com tipagem estrita no Pydantic e controle de autenticação stateless via tokens JWT assinados criptograficamente.

---

### 📬 Onde me encontrar

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/felipecamargosantos/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SEU_USUARIO)
