# Lucas Martins Ferreira

**Desenvolvedor Back-end | Python · Java · SQL · IA e Automação**

Engenharia de Software — Universidade de Vassouras (5º período) · Armação dos Búzios, RJ

[LinkedIn](https://www.linkedin.com/in/lucas-martins-450718286/) · [E-mail](mailto:lucas.martins.bz@gmail.com)

Desenvolvo sistemas para apoiar decisões de estoque, organizar dados e automatizar operações. Conduzo projetos da definição do problema à implementação, com testes e documentação das decisões técnicas.

## Linguagens e ferramentas

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" alt="Python" title="Python" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" alt="Java" title="Java" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/fastapi/fastapi-original.svg" alt="FastAPI" title="FastAPI" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/spring/spring-original.svg" alt="Spring Boot" title="Spring Boot" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" alt="PostgreSQL" title="PostgreSQL" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/sqlalchemy/sqlalchemy-original.svg" alt="SQLAlchemy" title="SQLAlchemy" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pandas/pandas-original.svg" alt="pandas" title="pandas" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/scikitlearn/scikitlearn-original.svg" alt="scikit-learn" title="scikit-learn" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/streamlit/streamlit-original.svg" alt="Streamlit" title="Streamlit" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg" alt="Docker" title="Docker" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" alt="Git" title="Git" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/githubactions/githubactions-original.svg" alt="GitHub Actions" title="GitHub Actions" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pytest/pytest-original.svg" alt="pytest" title="pytest" width="36" height="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/ubuntu/ubuntu-original.svg" alt="Ubuntu Server" title="Ubuntu Server" width="36" height="36" />
</p>

- **Linguagens:** Python · Java · SQL · HTML · CSS · JavaScript.
- **Back-end e APIs:** FastAPI · Pydantic · Uvicorn · Spring Boot · Spring Data JPA · APIs REST.
- **Dados e persistência:** PostgreSQL · pgvector · TimescaleDB · SQLAlchemy.
- **IA e aprendizado de máquina:** Ollama · RAG · embeddings · nomic-embed-text · Qwen 2.5 · scikit-learn · XGBoost · pandas.
- **Interfaces:** Streamlit · Tkinter.
- **Qualidade e entrega:** pytest · unittest · Ruff · Git · GitHub Actions · CI/CD.
- **Infraestrutura:** Docker · Docker Compose · Ubuntu Server · Tailscale · SSH · runner self-hosted.

## Resultados em destaque

- **Erro de previsão 83% menor que a referência semanal**, em benchmark com dados sintéticos: Random Forest com MAE de 0,533 un./dia contra 3,095, em três janelas temporais de teste. [Metodologia e limites](https://github.com/LucasSMFerreira/previsao-vendas-estoque/blob/main/docs/benchmark/README.md).
- **Quatro projetos públicos em back-end, automação e IA**, incluindo um assistente RAG com modelos locais, aplicações de estoque e uma API Java.
- **Segurança implementada na aplicação de previsão:** scrypt com salt individual, bloqueio após cinco tentativas e expiração de sessão por inatividade.
- **Integração contínua com banco real:** testes de inicialização, isolamento de contas e importação idempotente em PostgreSQL/TimescaleDB descartável no GitHub Actions.

## Projetos-chave

### [Assistente de Estudos com IA](https://github.com/LucasSMFerreira/assistente-estudos)

**Objetivo:** consultar PDFs de aula por perguntas em linguagem natural, com indicação do documento e da página.

- Implementei um fluxo RAG com ingestão de PDFs, embeddings e busca vetorial no PostgreSQL com pgvector, integrado a modelos locais pelo Ollama.
- Comparei quatro configurações de divisão de texto em um conjunto de 15 perguntas: o baseline alcançou Acerto@4 de 73,3% e MRR de 0,70. A avaliação é pequena e mede a recuperação das fontes, não a precisão final das respostas.
- Estruturei CI com Ruff e pytest e deploy automatizado em servidor Ubuntu próprio, com Docker e runner self-hosted.

**Stack:** Python · FastAPI · Pydantic · Uvicorn · PostgreSQL · pgvector · SQLAlchemy · Ollama · Docker Compose · pytest · Ruff · GitHub Actions · Ubuntu Server · Tailscale.

**Limite atual:** respostas levam de 1 a 3 minutos no hardware local sem GPU, conforme a documentação do projeto.


### [Previsão de Demanda e Planejamento de Estoque](https://github.com/LucasSMFerreira/previsao-vendas-estoque)

**Objetivo:** transformar registros de vendas em estimativas de demanda e apoio à reposição.

- Desenvolvi uma aplicação multiusuário para registrar vendas, comparar previsões e estimar reposição, com dados separados por conta.
- Comparei referência semanal, Random Forest e XGBoost em avaliação temporal; o Random Forest reduziu o MAE em aproximadamente 83% no cenário sintético. O resultado não representa precisão validada em vendas reais.
- Estruturei testes automatizados, CI com banco descartável e documentação de atualização para a versão 1.0.

**Stack:** Python · scikit-learn · XGBoost · SQLAlchemy · PostgreSQL/TimescaleDB · Streamlit · Docker · pytest · GitHub Actions.

### [Planejamento de Reposição de Estoque](https://github.com/LucasSMFerreira/reposicao-estoque)

**Objetivo:** calcular quando e quanto comprar, considerando prazo de entrega e restrições do fornecedor.

- Separei regras de negócio, interface e persistência para facilitar manutenção e evolução.
- Implementei ajuste à compra mínima e ao múltiplo do fornecedor, com registro das decisões de aceitar, ajustar ou adiar.
- Entreguei interface desktop e opção por terminal, com testes e sem dependências externas à biblioteca padrão do Python.

**Stack:** Python · Tkinter · JSON · CSV · unittest.

### [Data Remo API](https://github.com/LucasSMFerreira/data-remo-api)

**Objetivo:** organizar o histórico de atletas, treinos e indicadores de desempenho no remo.

- Estruturei 11 endpoints para cadastro, consultas por período, ranking e resumo mensal.
- Organizei o código em controllers, serviços, repositórios e DTOs, com persistência relacional.
- Apliquei Factory, Observer e Decorator em exercícios do domínio.

**Stack:** Java 21 · Spring Boot · Spring Data JPA · PostgreSQL · Maven.

**Estágio:** protótipo acadêmico; autenticação das rotas, migrações e testes funcionais são evoluções pendentes.

## Liderança e iniciativa

- **Fundador da SmartShop:** defini proposta de produto, modelo de assinatura e preços para uma comunidade e loja de ferramentas digitais.
- **Criador do Orquestra:** conduzo concepção, desenvolvimento, distribuição e suporte de uma ferramenta de geração de sites em volume com IA.
- **Automação de operações:** implementei bots em nuvem para automatizar venda e entrega, dispensando intervenção manual por pedido.
- **Organização de entregas:** formação certificada em Scrum, com foco em priorização e evolução incremental.

---

Aberto a oportunidades em **back-end, automação e IA**.
