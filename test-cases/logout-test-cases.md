# Módulo de Logout – Casos de Teste

**Sistema:** OrangeHRM Demo  
**Módulo:** Logout  
**Testador:** Ruan Almeida  
**Navegador:** Google Chrome  
**Sistema Operacional:** Windows  
**Data:** 28/02/2026  

---

## TC-LOGOUT-001 – Verificar invalidação de sessão ao utilizar botão voltar do navegador após logout

**Tipo:** Segurança  

**Prioridade:** Baixa  

### Pré-condição
Usuário autenticado no sistema com sessão ativa e Dashboard carregado.

### Passos para execução
1. Realizar login com credenciais válidas.
2. Confirmar acesso ao Dashboard.
3. Clicar na opção "Logout".
4. Na tela de login, clicar no botão "Voltar" (←) do navegador.
5. Observar o comportamento da aplicação.

### Resultado Esperado
Após o logout, o sistema não deve permitir a visualização de páginas internas, mesmo utilizando o botão voltar do navegador.

O usuário deve permanecer na tela de login e qualquer tentativa de acesso à URL interna deve ser bloqueada imediatamente.

### Resultado Obtido
Ao clicar no botão voltar após o logout:
- O Dashboard é exibido novamente.
- A URL interna é carregada.
- Ao interagir com qualquer funcionalidade, o sistema redireciona o usuário para a tela de login.

### Status
Failed

Relação com Bugs
TC-LOGOUT-001 → BUG-LOGOUT-001 (Status: Failed)
