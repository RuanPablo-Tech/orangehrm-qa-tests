🐞 # BUG-LOGOUT-001 — Logout permite retorno visual ao Dashboard via botão Voltar

Pré-condição
Usuário autenticado no sistema
Acesso ao Dashboard
Sessão ativa

Passos para reprodução
Realizar login com usuário válido
Acessar o Dashboard
Clicar em Logout
Na tela de login, clicar no botão Voltar (←) do navegador

Resultado esperado
Após o logout, o usuário não deve conseguir visualizar páginas internas do sistema, mesmo utilizando o botão Voltar do navegador.
O sistema deve bloquear o acesso e manter o usuário na tela de login.

Resultado obtido
Ao clicar no botão Voltar do navegador após o logout:
O sistema exibe novamente o Dashboard
A URL correspondente à área interna é carregada
Ao tentar interagir com qualquer item do menu, o sistema redireciona o usuário para a tela de login.

Observação
O conteúdo do Dashboard aparenta estar sendo carregado a partir de cache do navegador, permitindo visualização momentânea da interface mesmo com a sessão encerrada.

Severidade
🟡 Baixa
Apesar da visualização do Dashboard, o sistema bloqueia qualquer interação e redireciona para a tela de login ao tentar acessar funcionalidades internas.

Evidência

### Evidências

- ![Dashboard visível após logout](evidences/bug-logout-001-dashboard-after-logout.png)
- ![Retorno ao Dashboard via botão Voltar](evidences/bug-logout-001-back-button-dashboard.png)
