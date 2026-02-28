# 🐞 Bug Report

## Título
Logout permite retorno visual ao dashboard ao utilizar botão voltar do navegador

## Tipo
Segurança

## Ambiente
- URL: https://opensource-demo.orangehrmlive.com
- Ambiente: Produção (Demo pública)
- Navegador: Chrome
- Sistema Operacional: Windows

## Pré-condição
- Usuário autenticado no sistema
- Sessão ativa
- Dashboard carregada corretamente

## Passos para reprodução
1. Realizar login com usuário válido
2. Acessar o dashboard
3. Clicar em logout
4. Na tela de login, clicar no botão voltar (←) do navegador

## Resultado esperado
Após o logout, o sitema não deve permitir a vizualização de páginas internas, mesmo ao utilizar o botão voltar do navegador

O usuário deve permanecer na tela de login e qualuqer tentativa de acesso à URL interna deve ser bloqueada imediatamente

## Resultado real
Ao clicar no botão voltar após o logout:
- O dashboard é exibido novamente
- A URL da área interna é carregada
- Ao interagir com qualquer funcionalidade, o sistema redireciona o usuário para a tela de login

## Severidade
Baixa

## Evidência
- ![Dashboard visível após logout](evidences/bug-logout-001-dashboard-after-logout.png)

- ![Retorno ao Dashboard via botão Voltar](evidences/bug-logout-001-back-button-dashboard.png)

