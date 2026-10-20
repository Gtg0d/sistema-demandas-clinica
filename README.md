# Sistema de Demandas da Clínica

Sistema web interno que uso no meu trabalho para organizar as demandas da equipe de uma clínica de reabilitação: quem pediu, quem faz, prazo, andamento e histórico, tudo em tempo real.

> O código é privado porque roda em produção com dados reais. Este repositório mostra o projeto, as decisões e o que aprendi.

## O problema
As demandas chegavam por WhatsApp, papel e boca a boca. Coisa se perdia, ninguém sabia o status e não havia histórico.

## O que o sistema faz
- Criar, distribuir e acompanhar demandas, com atualização em tempo real (Socket.io)
- Checklist dentro de cada demanda
- Demandas sigilosas e demandas fixas
- Página de administração de usuários e perfis de acesso
- Histórico com exportação para Excel
- PWA: instala no celular e manda notificação de nova demanda
- Visual configurável dos cards (Compacto/Clássico)

## Stack
Node.js · Express · PostgreSQL · Socket.io · Web Push / PWA · HTML, CSS e JavaScript · Deploy no Railway

## Prints
Em breve (com dados fictícios).

## Como evoluiu
- **v1:** primeira versão, resolveu o básico
- **v2:** revisão de segurança, interface nova, PWA com notificações, checklist, administração de usuários, exportação Excel, dependências sem alertas (`npm audit`: 0)
- Deploy com ambiente de staging antes de produção e plano de rollback

## O que aprendi
- Modelar banco relacional e escrever SQL de verdade
- Tempo real com WebSockets
- Segurança básica de aplicação web: autenticação, permissões, dependências
- Deploy, variáveis de ambiente e rollback em produção
- Usar IA (Claude Code) como par de programação, revisando o que ela escreve
- Ouvir usuários de verdade e transformar pedido em funcionalidade
