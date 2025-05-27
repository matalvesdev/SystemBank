
# 💳 Sistema Bancário Simplificado

Este é um projeto prático desenvolvido em Java para simular operações bancárias básicas. O objetivo foi consolidar os principais conceitos da linguagem de forma objetiva.

---

## 🚀 Funcionalidades

- Criação de contas correntes  
- Depósito, saque e transferência entre contas  
- Visualização de saldo  
- Validações de saldo e valores inseridos

---

## 🛠️ Estrutura Principal

### Classe: `ContaCorrente`

**Atributos:**

| Atributo   | Descrição                        |
|------------|----------------------------------|
| `cpf`      | Identificador único da conta     |
| `nome`     | Nome do titular da conta         |
| `saldo`    | Valor disponível na conta        |

**Métodos:**

- `sacar(double valor)`  
  Realiza um saque após validar se há saldo suficiente.

- `depositar(double valor)`  
  Adiciona o valor ao saldo, validando se o valor informado é positivo.

- `transferir(ContaCorrente contaDestino, double valor)`  
  Transfere valores entre contas, sempre validando o saldo antes.

- `verSaldo()`  
  Retorna o saldo atual da conta.

---

## 💡 Exemplos de Uso

```java
ContaCorrente contaMateus = new ContaCorrente("12345678901", "Mateus", 1000.0);
ContaCorrente contaFlor = new ContaCorrente("10987654321", "Flor", 500.0);

contaMateus.sacar(200.0);
contaMateus.depositar(300.0);
contaMateus.transferir(contaFlor, 150.0);

System.out.println("Saldo Mateus: " + contaMateus.verSaldo());
System.out.println("Saldo Flor: " + contaFlor.verSaldo());
```

---

## 📚 O que aprendi

- Aplicar encapsulamento e proteger atributos
- Criar e utilizar métodos e construtores
- Promover a integração entre objetos
- Realizar testes básicos de operações

---

## ▶️ Como executar

1. Clone este repositório:
   ```sh
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Compile o projeto com o Maven ou diretamente pela sua IDE.
3. Execute a classe Main para simular as operações.

---

## 🏁 Objetivo

Meu objetivo com este projeto foi me tornar capaz de criar e manipular classes em Java, simulando um sistema bancário realista e funcional.

Projeto desenvolvido com fins didáticos e para prática de programação orientada a objetos em Java.

---
