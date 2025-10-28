# banco-digital

Olá — este repositório contém um projeto pessoal que desenvolvi para estudar e praticar conceitos fundamentais de engenharia de software com Python. O objetivo principal foi construir um sistema bancário simples, porém bem modelado, que demonstre claramente minhas escolhas de design, organização e atenção à qualidade de código.

## Sobre o projeto

Criei esta mini-aplicação para exercitar: modelagem de domínio usando programação orientada a objetos, separação de responsabilidades, tratamento explícito de erros e escrita de código testável e legível. A aplicação cobre operações bancárias básicas (criação de clientes e contas, depósito, saque e transferência) e foi organizada em pacotes para refletir uma arquitetura em camadas clara.

Este projeto é ideal para decisões de design, trade-offs e uma possível evolução da solução para um contexto real (persistência, API, autenticação, escalabilidade).

## Tecnologias e práticas aplicadas

- Linguagem: Python 3.8+
- Arquitetura: organização em pacotes (`entidades/`, `operacoes/`, `utilitarios/`) com responsabilidades separadas
- Paradigma: Programação Orientada a Objetos (encapsulamento, responsabilidades únicas, métodos claros)
- Tratamento de erros: exceções customizadas para cenários de negócio (ex.: saldo insuficiente)
- Boas práticas: código modular, nomes e docstrings descritivos, projeto pensado para testabilidade
- Controle de versão: uso previsto de Git (fluxo de branches e PRs recomendado)

Obs.: o projeto foi criado como exercício didático e, por isso, não depende de pacotes externos — a intenção é demonstrar clareza de código sem camadas adicionais.

## Estrutura do repositório

- `app.py` — exemplo simples de execução do fluxo (ponto de entrada)
- `entidades/` — modelos de domínio (por exemplo, `cliente.py`, `conta.py`)
- `operacoes/` — regras de negócio e orquestração (por exemplo, `banco.py`)
- `utilitarios/` — exceções e utilitários auxiliares (`exceptions.py`)
- `README.md`, `LICENSE` — documentação e licença

Essa separação torna o código fácil de revisar e estender: modelos contêm apenas dados e validações, enquanto a camada de operações implementa regras e políticas.

## Por que escolhi fazer este projeto?

1. Demonstra habilidade com modelagem e design (OOP).
2. Mostra entendimento de separação de responsabilidades e código testável.
3. Permite discutir como transformar um protótipo em um serviço de produção (persistência, API, testes, CI/CD).
4. Código simples, mas intencional — facilita analises técnicas e revisões.

## Como executar

Recomendo usar um ambiente virtual local para reprodução. Abaixo está o fluxo no PowerShell (Windows):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python app.py
```
