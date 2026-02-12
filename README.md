```markdown
# ⚖️ RAG Jurídico — CDC & LGPD

Projeto desenvolvido durante a Sprint 1 do programa **#6 Conecta+ | Agentes de IA para Dev**  
Alura — Cursos Online de Tecnologia  
Período: 02/02/2026 a 13/02/2026  
Aluna: **Mirian Ajiki Molicawa**

---

## 📌 Sobre o Projeto

Este projeto implementa uma aplicação baseada em **RAG (Retrieval-Augmented Generation)**
 aplicada ao domínio jurídico, utilizando como base:

- 📘 Código de Defesa do Consumidor (CDC)
- 🔐 Lei Geral de Proteção de Dados (LGPD)

O sistema permite realizar consultas em linguagem natural e obter respostas fundamentadas nos documentos legais indexados.

---

## 🎯 Objetivo

Construir um sistema capaz de:

- 📄 Indexar documentos jurídicos em PDF
- 🔎 Realizar busca semântica com embeddings
- 🤖 Utilizar LLM para geração de respostas contextualizadas
- ⚖️ Auxiliar na análise e interpretação de textos legais

---

## 🧠 Arquitetura da Solução

O fluxo da aplicação segue o padrão RAG:

1. **Ingestão dos PDFs**
2. Extração e fragmentação (chunking)
3. Geração de embeddings
4. Armazenamento em banco vetorial (Chroma)
5. Consulta semântica
6. Geração de resposta com LLM utilizando contexto recuperado

---

## 🛠️ Tecnologias Utilizadas

- Python
- LangChain
- OpenAI API
- ChatOpenAI
- ChromaDB (Vector Store)
- Streamlit (Interface)
- PyPDF Loader
- HuggingFace

---

## 📂 Estrutura do Projeto

rag-juridico/
│
├── dados/
│   ├── cdc.pdf
│   └── lgpd.pdf
│
├── ingestao.py   # Pipeline de ingestão e vetorização
├── rag.py        # Lógica de recuperação + geração
├── app.py        # Interface Streamlit
└── README.md


---

## ⚙️ Pré-requisitos

Certifique-se de ter:

- Python 3.9+
- Chave da OpenAI configurada
- Loader de PDF funcionando
- Banco vetorial Chroma configurado

---

## 🚀 Como Executar

### 1️⃣ Clone o repositório

```bash
git clone https://github.com/ajikisan/rag-juridico.git
cd rag-juridico
````

### 2️⃣ Instale as dependências

```bash
pip install -r 
```

### 3️⃣ Configure sua variável de ambiente

```bash
export OPENAI_API_KEY="sua_chave_aqui"

```

### 4️⃣ Execute a aplicação

```bash
streamlit run app.py
```

---

## 💡 Aplicabilidade

Esta solução pode ser utilizada para:
* Assistentes jurídicos internos
* Apoio a times de compliance
* Consulta automatizada de legislação
* Base para LegalTechs
* Estudos de IA aplicada ao Direito

---

## 📚 Status do Projeto

✅ Sprint concluída
⚠️ Limitação de tokens durante testes com LLM
🔄 Possível evolução futura com otimização de chunks e modelo

---

## 👩🏻‍💻 Autora

Mirian Ajiki Molicawa
Desenvolvedora com foco em IA aplicada a negócios e produtos digitais

