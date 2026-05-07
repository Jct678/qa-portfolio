# Casos de Teste

---

## CT01 - Pagamento com cartão válido

### Entrada
- Dados válidos de cartão de crédito
- Data futura
- CVV válido

### Passos
1. Acessar a aba "Seus pagamentos"
2. Selecionar "Adicionar cartão"
3. Preencher os dados do cartão
4. Clicar em "Adicionar cartão"

### Resultado Esperado
Cartão cadastrado e pagamento processado com sucesso

---

## CT02 - Pagamento com cartão expirado

### Entrada
- Nome do cartão válido
- Número do cartão válido
- Data de expiração inválida
- CVV válido

### Passos
1. Acessar a área de pagamentos
2. Selecionar "Adicionar cartão"
3. Inserir os dados do cartão
4. Clicar em "Adicionar cartão"

### Resultado Esperado
Sistema deve impedir o cadastro do cartão e exibir mensagem de data inválida

---

## CT03 - Pagamento duplicado

### Entrada
- Pagamento via cartão aprovado
- Pedido não exibido na aba "Pedidos"
- Novo pagamento realizado via PIX

### Passos
1. Realizar pagamento via cartão
2. Confirmar aprovação do pagamento
3. Verificar ausência do pedido
4. Realizar novo pagamento via PIX

### Resultado Esperado
Sistema deve identificar pagamento duplicado e impedir a criação de pedidos duplicados
