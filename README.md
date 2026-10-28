# Lucas Martins Ferreira

**Desenvolvedor Back-end | Python · Java · SQL · IA e Automação**

Engenharia de Software — Universidade de Vassouras (5º período) · Armação dos Búzios, RJ

[LinkedIn](https://www.linkedin.com/in/lucas-martins-450718286/) · [E-mail](mailto:lucas.martins.bz@gmail.com)

Desenvolvo sistemas para apoiar decisões de estoque, organizar dados e automatizar operações. Conduzo projetos da definição do problema à implementação, com testes e documentação das decisões técnicas.

## Resultados em destaque

- **Erro de previsão 83% menor que a referência semanal**, em benchmark com dados sintéticos: Random Forest com MAE de 0,533 un./dia contra 3,095, em três janelas temporais de teste. [Metodologia e limites](https://github.com/LucasSMFerreira/previsao-vendas-estoque/blob/main/docs/benchmark/README.md).
- **Três projetos públicos em back-end, dados e estoque**, com persistência, regras de negócio e documentação: uma aplicação web local, uma aplicação desktop e uma API REST.
- **Segurança implementada na aplicação de previsão:** scrypt com salt individual, bloqueio após cinco tentativas e expiração de sessão por inatividade.
- **Integração contínua com banco real:** testes de inicialização, isolamento de contas e importação idempotente em PostgreSQL/TimescaleDB descartável no GitHub Actions.

## Projetos-chave

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

## Stack

- **Linguagens:** Python · Java · SQL.
- **Back-end e dados:** Spring Boot · Flask · APIs REST · PostgreSQL · TimescaleDB · SQLAlchemy.
- **IA e ML:** scikit-learn · XGBoost · pandas · IA generativa · agentes de IA.
- **Qualidade e entrega:** pytest · unittest · GitHub Actions · Docker · Git.

---

Aberto a oportunidades em **back-end, automação e IA**.
