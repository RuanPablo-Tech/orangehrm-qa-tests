# Módulo de Login – Casos de Teste

**Sistema:** OrangeHRM Demo  
**Módulo:** Login  
**Testador:** Ruan Almeida  
**Navegador:** Google Chrome  
**Sistema Operacional:** Windows  
**Data:** 28/02/2026  

---

## TC-LOGIN-001 – Login com credenciais válidas

**Tipo:** Funcional 

**Prioridade:** Alta  

### Pré-condição
Usuário cadastrado no sistema e deslogado.

### Passos para execução
1. Inserir username válido  
2. Inserir senha válida  
3. Clicar no botão "Login"  

### Resultado Esperado
O usuário deve ser redirecionado para o Dashboard do sistema.

### Status
Passed

---

## TC-LOGIN-002 – Tentativa de login com senha inválida

**Tipo:** Negativo  

**Prioridade:** Alta  

### Pré-condição
Página de login carregada corretamente.

### Passos para execução
1. Inserir username válido  
2. Inserir senha inválida  
3. Clicar no botão "Login"  

### Resultado Esperado
O sistema deve exibir a mensagem "Invalid credentials" e impedir o acesso ao sistema.

### Status
Passed

---

## TC-LOGIN-003 – Verificar consistência das mensagens de erro para login inválido

**Tipo:** UX / Validação  

**Prioridade:** Baixa  

### Pré-condição
Usuário está na tela de login com a página carregada corretamente.

### Passos para execução
1. Deixar o campo Username vazio e preencher o campo Password com valor válido.
2. Clicar no botão "Login".
3. Registrar a mensagem exibida.
4. Inserir Username inválido e Password inválido.
5. Clicar no botão "Login".
6. Comparar as mensagens apresentadas nas duas tentativas.

### Resultado Esperado
O sistema deve exibir mensagens de erro padronizadas e consistentes para todas as tentativas inválidas de login, garantindo padronização na comunicação de erro.

### Resultado Obtido
Mensagens diferentes são exibidas dependendo da combinação de dados inválidos.

### Status
Failed

## Relação com Bugs

TC-LOGIN-003 → BUG-LOGIN-001 (Status: Failed)
