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

---

## CT04 - Pagamento com CVV inválido

### Entrada
- Número do cartão válido
- Data de expiração válida
- CVV inválido

### Passos
1. Acessar a área de pagamentos
2. Selecionar "Adicionar cartão"
3. Inserir os dados do cartão
4. Informar CVV inválido
5. Clicar em "Adicionar cartão"

### Resultado Esperado
Sistema deve impedir o pagamento e exibir mensagem de CVV inválido

---

## CT05 - Campo obrigatório vazio

### Entrada
- Campo número do cartão vazio
- Nome válido
- Data válida
- CVV válido

### Passos
1. Acessar a área de pagamentos
2. Selecionar "Adicionar cartão"
3. Deixar o campo número do cartão vazio
4. Preencher os demais campos
5. Clicar em "Adicionar cartão"

### Resultado Esperado
Sistema deve impedir o cadastro e informar campo obrigatório

---

## CT06 - PIX expirado

### Entrada
- QR Code PIX expirado

### Passos
1. Selecionar pagamento via PIX
2. Aguardar expiração do QR Code
3. Tentar concluir o pagamento

### Resultado Esperado
Sistema deve informar que o QR Code expirou e gerar um novo código PIX

---

## CT07 - Interrupção de internet durante pagamento

### Entrada
- Pagamento iniciado com conexão interrompida durante processamento

### Passos
1. Adicionar produto ao carrinho
2. Selecionar pagamento via cartão
3. Confirmar pagamento
4. Interromper conexão com internet durante processamento

### Resultado Esperado
Sistema deve informar falha na conexão e impedir cobrança duplicada

---

## CT08 - Pagamento com saldo insuficiente

### Entrada
- Cartão com saldo insuficiente

### Passos
1. Acessar área de pagamentos
2. Inserir dados do cartão
3. Confirmar pagamento

### Resultado Esperado
Sistema deve recusar o pagamento e exibir mensagem de saldo insuficiente
