# 🧪 Projeto QA - Sistema de Pagamento Amazon

## 📌 Sobre o Projeto
Este projeto foi desenvolvido com foco em testes manuais de um sistema de pagamentos inspirado no fluxo da Amazon.

O objetivo é validar diferentes métodos de pagamento, identificar falhas no sistema e documentar cenários reais de teste utilizados em QA Manual.

---

# 🎯 Objetivo
Validar o funcionamento dos métodos de pagamento e garantir que o sistema aceite apenas transações válidas.

---

# 🔍 Escopo dos Testes

Os seguintes métodos de pagamento foram analisados:

- PIX
- Cartão de crédito
- Boleto
- NuPay
- Geru

---

# 🚫 Fora do Escopo

Os seguintes módulos não fazem parte deste projeto:

- Endereço
- Frete
- Rastreamento de pedidos

---

# 🧠 Estratégia de Teste

Os testes foram realizados utilizando:

- Testes manuais
- Dados válidos e inválidos
- Validação de campos obrigatórios
- Testes de comportamento inesperado
- Simulação de falhas reais

---

# 🧪 Cenários Testados

- Pagamento com cartão válido
- Cartão expirado
- CVV inválido
- Campo obrigatório vazio
- PIX expirado
- Pagamento duplicado
- Internet interrompida durante pagamento
- Saldo insuficiente

---

# 🐞 Bugs Identificados

- Sistema permite pagamento duplicado
- Sistema aceita cartão expirado

---

# 📊 Resultado Final

O sistema apresentou falhas importantes relacionadas à validação de pagamentos e prevenção de duplicidade.

As inconsistências identificadas podem impactar diretamente a experiência do usuário e a segurança das transações.

---

# 🛠️ Ferramentas Utilizadas

- GitHub
- Markdown
- Testes Manuais

---

# 📁 Estrutura do Projeto

```text
amazon-payment-tests
├── README.md
├── casos-de-teste.md
├── bugs.md
└── relatorio-final.md
```

---

# ✅ Status do Projeto

✔ Em desenvolvimento
