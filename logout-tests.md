# Logout – Testes Manuais

## Objetivo
Validar que o logout encerra corretamente a sessão do usuário e impede o acesso a áreas internas do sistema.

---

## CT-LOGOUT-01 – Logout com sucesso
Pré-condição:
Usuário autenticado no sistema

Passos:
1. Clicar no menu do usuário
2. Selecionar "Logout"

Resultado esperado:
Usuário é redirecionado para a tela de login

---

## CT-LOGOUT-02 – Acesso via botão Voltar após logout
Pré-condição:
Usuário realizou logout

Passos:
1. Clicar no botão Voltar do navegador

Resultado esperado:
Usuário não deve visualizar páginas internas do sistema
