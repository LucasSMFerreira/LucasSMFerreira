# Lucas Martins Ferreira

Desenvolvedor em formação, com estudos em Java, Python, Node.js, SQL e desenvolvimento web.
Compartilho projetos acadêmicos e pessoais, com foco em entender as decisões do código e evoluir com testes e documentação.

## Projetos em destaque

| Projeto | O que você encontra | Tecnologias |
|---|---|---|
| [Previsão de demanda e estoque](https://github.com/LucasSMFerreira/Previsao-demanda-estoque) | Cadastro de lojas e produtos, vendas, previsão e apoio à reposição. Edição local com testes e comparação temporal de modelos. | Python, Streamlit, PostgreSQL, TimescaleDB |
| [Reposição automática de estoque](https://github.com/LucasSMFerreira/Reposi-o-Automatica-Estoque) | Painel leve para acompanhar prioridades, calcular compras sugeridas e registrar decisões. | Python, Tkinter, CSV/JSON |
| [Compras e Fornecedores](https://github.com/LucasSMFerreira/Compra-Fornecedores) | Pedidos de compra com aprovação, fornecedor, envio à API de Contas e registro de entrega. Exemplos isolados dos dados reais. | Python, Tkinter, JSON, API local |
| [Contas a Pagar](https://github.com/LucasSMFerreira/Controle-Contas) | Vencimentos, contas recorrentes, comprovantes e API local para compras aprovadas. | Python, Tkinter, JSON, API local |
| [Clínica veterinária](https://github.com/LucasSMFerreira/Sistema-de-Clinica-Veterinaria) | Estudo de atendimento veterinário aplicando State, Observer e Decorator. | Java, orientação a objetos |
| [Site para nutricionista](https://github.com/LucasSMFerreira/LandingPageNutri) | Site institucional com apresentação, serviços e contato. | HTML, CSS, interface responsiva |

## Projetos conectados

Os quatro projetos funcionam separadamente e foram preparados como módulos de uma aplicação final de gestão:

1. [Previsão de Demanda](https://github.com/LucasSMFerreira/Previsao-demanda-estoque) estima o consumo futuro. A saída ainda não entra automaticamente na Reposição.
2. [Reposição Automática de Estoque](https://github.com/LucasSMFerreira/Reposi-o-Automatica-Estoque) calcula a necessidade de compra e registra a decisão de aceitar, ajustar ou adiar.
3. [Compras e Fornecedores](https://github.com/LucasSMFerreira/Compra-Fornecedores) importa decisões aprovadas do JSON de produtos e do CSV de decisões, cria pedidos, exige conferência e acompanha a entrega.
4. [Contas a Pagar](https://github.com/LucasSMFerreira/Controle-Contas) recebe, pela API local, o pedido aprovado com preço e vencimento e cria a conta financeira.

```text
Previsão (estimativa) → Reposição (decisão) → Compras (pedido) → Contas (despesa)
                              JSON + CSV              API HTTP local
```

Para usar a ponte, ative **Ativar ponte** em Contas a Pagar e, em Compras, selecione um pedido aprovado e clique em **Criar conta a pagar**. O envio é um `POST /api/v1/pedidos-reposicao` para `127.0.0.1:8765` com número do pedido, SKU, produto, fornecedor, quantidade, preço unitário e vencimento. A resposta traz o identificador da conta. O número do pedido impede criar outra conta ao repetir o envio. O recebimento fica registrado em Compras; a entrada automática no estoque ainda está pendente. A Reposição também permite envio direto ao Contas, mas o fluxo pelo módulo de Compras concentra o acompanhamento do pedido.

## Estudos de Python

- [Sistema bancário](https://github.com/LucasSMFerreira/SistemaBancario)
- [Folha de pagamento](https://github.com/LucasSMFerreira/SistemaFolhadePagamento)
- [Biblioteca](https://github.com/LucasSMFerreira/Biblioteca)
- [Sistema de loja](https://github.com/LucasSMFerreira/SistemaLoja)

## Estudos de padrões de projeto

Exercícios separados por padrão para facilitar a consulta:

- Criação: [Factory Method](https://github.com/LucasSMFerreira/Padrao-FactoryMethod), [Abstract Factory](https://github.com/LucasSMFerreira/Padrao-AbstractFactory) e [Singleton](https://github.com/LucasSMFerreira/Padrao-Singleton).
- Estrutura: [Bridge](https://github.com/LucasSMFerreira/Padrao-Brigde) e [Decorator](https://github.com/LucasSMFerreira/Padrao-Decorator).
- Comportamento: [Observer](https://github.com/LucasSMFerreira/Padr-o-Observer), [Strategy](https://github.com/LucasSMFerreira/Padrao-Strategy), [State](https://github.com/LucasSMFerreira/PadraoState), [Chain of Responsibility](https://github.com/LucasSMFerreira/Padrao-Chain-of-responsibility) e [Template Method](https://github.com/LucasSMFerreira/TemplateMethod).

## Contato

[LinkedIn](https://www.linkedin.com/in/lucas-martins-450718286/)
