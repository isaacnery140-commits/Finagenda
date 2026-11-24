# Finagenda: agenda e gastos

App para celular com **agenda** e **controle de gastos**. Para cada pessoa, você escolhe o que compartilhar: só a agenda, só os gastos ou os dois.

- **Endereço:** https://finagenda.com.br (GitHub Pages, branch `main`, raiz; arquivo `CNAME`)
- **Play Store:** pacote `br.com.finagenda.app`, gerado pelo PWABuilder (TWA)
- **Banco:** Supabase, projeto `pvhoumlovxjlqvmchobv`. As tabelas e funções começam com `juntos_`, o nome antigo do app; o SQL está em `supabase/`.
- **Notificações:** Edge Function `juntos-push` (`supabase/functions/juntos-push`), chamada pelos gatilhos do banco e pela tarefa `juntos-lembretes`.

## Páginas públicas
- `termos.html` (Termos de uso)
- `privacidade.html` (Política de privacidade)
- `suporte.html` (Ajuda e suporte)
- `excluir-conta.html` (excluir a conta pela internet)

## Publicar uma atualização
1. Altere os arquivos e aumente `VERSAO` no `index.html` e `CACHE` no `sw.js`.
2. Faça commit e push na `main`. O GitHub Pages publica sozinho.
