# Lab Padrões de Projeto com Java

Implementação dos principais padrões de projeto (Design Patterns) utilizando Java, desenvolvida a partir do laboratório da Digital Innovation One (DIO).

## Sobre o projeto

Este projeto demonstra a aplicação prática de alguns dos padrões de projeto mais conhecidos da programação orientada a objetos, conforme descritos pelo GoF (Gang of Four).

O objetivo é apresentar exemplos simples e didáticos dos padrões:

* Singleton
* Strategy
* Facade

Cada implementação busca demonstrar o propósito do padrão, sua estrutura e o problema que ele resolve.

## Padrões implementados

### Singleton

Garante que uma classe possua apenas uma única instância durante todo o ciclo de vida da aplicação.

Implementações presentes:

* Singleton Lazy
* Singleton Eager
* Singleton Lazy Holder

Arquivos:

```text
singleton/
├── SingletonLazy.java
├── SingletonEager.java
└── SingletonLazyHolder.java
```

### Strategy

Permite definir uma família de algoritmos, encapsulá-los e torná-los intercambiáveis em tempo de execução.

Neste exemplo, um robô pode alterar seu comportamento dinamicamente.

Comportamentos disponíveis:

* Normal
* Defensivo
* Agressivo

Arquivos:

```text
strategy/
├── Comportamento.java
├── ComportamentoNormal.java
├── ComportamentoDefensivo.java
├── ComportamentoAgressivo.java
└── Robo.java
```

### Facade

Fornece uma interface simplificada para um conjunto de subsistemas complexos.

Neste exemplo, a fachada centraliza a comunicação entre:

* Sistema de CRM
* Serviço de CEP

Arquivos:

```text
facade/
└── Facade.java

subsistema1/
└── crm/

subsistema2/
└── cep/
```

## Estrutura do projeto

```text
src/
├── one/
│   └── digitalinnovation/
│       └── gof/
│           ├── facade/
│           ├── singleton/
│           ├── strategy/
│           └── Test.java
├── subsistema1/
│   └── crm/
└── subsistema2/
    └── cep/
```

## Tecnologias utilizadas

* Java
* Programação Orientada a Objetos (POO)
* Design Patterns (GoF)
* Git
* GitHub

## Como executar

Compile os arquivos:

```bash
javac -d out $(find src -name "*.java")
```

Execute a classe principal:

```bash
java -cp out one.digitalinnovation.gof.Test
```

## Conceitos abordados

* Encapsulamento
* Polimorfismo
* Composição
* Inversão de comportamento
* Separação de responsabilidades
* Baixo acoplamento
* Reutilização de código

## Melhorias futuras

* Atualização para Java 21
* Uso de recursos modernos da linguagem
* Refatoração da estrutura dos pacotes
* Inclusão de testes automatizados
* Exemplos adicionais de padrões GoF

## Projeto original

Projeto desenvolvido a partir do laboratório "Explorando Padrões de Projetos na Prática com Java", disponibilizado pela Digital Innovation One (DIO).

## Licença

Projeto destinado a fins educacionais e de aprendizado.
