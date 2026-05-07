# Bugs Encontrados

---

## BUG01 - Sistema permite pagamento duplicado

### Descrição
Após um pagamento aprovado via cartão, o pedido não foi exibido na aba de pedidos. O usuário realizou um novo pagamento via PIX, gerando duplicidade de pagamento.

### Passos para reproduzir
1. Realizar pagamento via cartão
2. Confirmar aprovação do pagamento
3. Verificar ausência do pedido na aba "Pedidos"
4. Realizar novo pagamento via PIX

### Resultado Esperado
Sistema deve identificar pagamento já realizado e impedir novo pagamento duplicado.

### Resultado Atual
Sistema permitiu dois pagamentos para o mesmo pedido.

### Severidade
Alta

---

## BUG02 - Sistema aceita cartão expirado

### Descrição
O sistema permite cadastro de cartão com data de expiração inválida.

### Passos para reproduzir
1. Acessar área de pagamentos
2. Inserir cartão expirado
3. Confirmar cadastro

### Resultado Esperado
Sistema deve impedir cadastro do cartão e exibir mensagem de erro.

### Resultado Atual
Cartão expirado foi aceito pelo sistema.

### Severidade
Média
