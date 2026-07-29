# DFLINE CRM

Sistema interno (React via CDN + Babel in-browser, Firebase Firestore como banco de dados). Site estático de página única — sem build, sem dependências para instalar.

## Deploy

Este repositório é publicado no Netlify via deploy contínuo: todo push na branch `main` sobe automaticamente para produção. Não há passo de build — o Netlify só precisa servir `index.html`.

## Desenvolvimento

1. Edite `index.html` diretamente (ou peça pro Claude Code editar).
2. Para testar localmente antes de subir, basta abrir o arquivo num navegador (ou rodar `npx serve .` na pasta).
3. Abra um Pull Request para revisar as mudanças — o Netlify cria um **Deploy Preview** automático por PR, com uma URL própria para testar antes de ir pra produção.
4. Depois de aprovado, faça merge na `main` — o Netlify publica sozinho.

## Configuração

O projeto usa Firebase Firestore (config já embutido no `index.html`, é uma chave de cliente pública — a segurança real é feita pelas regras do Firestore, não pela chave em si).
