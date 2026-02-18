# 🏦 Sistema Bancário - Classes_M1

## Descrição Breve

Um projeto educacional em C# que demonstra os princípios fundamentais de Programação Orientada a Objetos. Implementa um sistema simples de gerenciamento bancário onde clientes podem abrir contas correntes/poupança com saldos personalizados. Cada cliente e conta recebem IDs/números únicos gerados automaticamente.

## 📋 Descrição Detalhada

Este projeto implementa um sistema básico de gerenciamento bancário com duas classes principais:

- **BankCustomer**: Representa um cliente do banco
- **BankAccount**: Representa uma conta bancária

## 🎯 Funcionalidades

### BankCustomer (Cliente Bancário)
- Geração automática de ID único para cada cliente
- Armazenamento de nome e sobrenome
- IDs gerados como números aleatórios de 10 dígitos
- Suporta dois tipos de construtor:
  - Construtor vazio (usa valores padrão: "Tim" e "Shao")
  - Construtor com parâmetros (nome e sobrenome personalizados)

### BankAccount (Conta Bancária)
- Geração automática de número único para cada conta
- Armazenamento de saldo inicial
- Tipos de conta (ex: "Checking")
- Taxa de juros estática compartilhada entre todas as contas
- Vinculação com ID do cliente
- Suporta dois tipos de construtor:
  - Construtor básico (apenas ID do cliente)
  - Construtor completo (ID do cliente, saldo inicial e tipo de conta)

## 🛠️ Estrutura do Projeto

```
Classes_M1\
├── Classes_M1.csproj       # Arquivo de configuração do projeto
├── Program.cs              # Programa principal com exemplos de uso
├── BankCustomer.cs         # Definição da classe BankCustomer
├── BankAccount.cs          # Definição da classe BankAccount
└── bin\                     # Artefatos compilados
```

## 🚀 Como Executar

1. Navegue até a pasta do projeto:
```bash
cd Classes_M1
```

2. Execute o projeto:
```bash
dotnet run
```

3. A saída exibirá informações sobre os clientes e conta criadas:
```
BankCustomer 1: Tim Shao [ID_DO_CLIENTE]
BankCustomer 2: Lisa Shao [ID_DO_CLIENTE]
BankCustomer 3: Sandy Zoeng [ID_DO_CLIENTE]
Account 1: Account # [NUMERO_CONTA], type Checking, balance 0, rate 0, customer ID [ID_CLIENTE]
Account 2: Account # [NUMERO_CONTA], type Checking, balance 1500, rate 0, customer ID [ID_CLIENTE]
Account 3: Account # [NUMERO_CONTA], type Checking, balance 2500, rate 0, customer ID [ID_CLIENTE]
```

## 💡 Conceitos de POO Demonstrados

- **Encapsulamento**: Uso de modificadores de acesso (public, private, readonly)
- **Classes Estáticas**: Variáveis estáticas para gerar IDs e números únicos
- **Construtores**: Múltiplos construtores (sobrecarga)
- **Atributos de Classe**: Campos estáticos compartilhados entre instâncias
- **Namespace**: Organização do código em namespaces

## 📦 Requisitos

- **.NET 10.0** ou superior
- C# 12 ou superior

## 📝 Notas

- Os IDs dos clientes e números de contas são gerados aleatoriamente na inicialização
- A taxa de juros (InterestRate) é uma propriedade estática compartilhada por todas as contas
- Os valores padrão para novos clientes são "Tim" e "Shao"

## 📚 Estrutura do Código

### BankCustomer.cs
Classe que representa um cliente bancário com ID único gerado automaticamente a partir de um valor aleatório entre 10 milhões e 20 milhões.

### BankAccount.cs
Classe que representa uma conta bancária vinculada a um cliente, com número de conta único e suporte a diferentes tipos de conta.

### Program.cs
Programa de demonstração que cria 3 clientes e 3 contas bancárias, exibindo suas informações no console.

---

**Desenvolvido como exercício de Programação Orientada a Objetos em C#**
