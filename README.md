# Kivitrine / G-Vitrine

Aplicação de vitrine de produtos multi-loja construída com TanStack Start, React, TypeScript e Supabase.

## Supabase configurado

- Projeto: `GVITRINE`
- Project ref: `jxyhzpvgihfkeduvomlu`
- URL: `https://jxyhzpvgihfkeduvomlu.supabase.co`

A aplicação usa `VITE_SUPABASE_URL` e `VITE_SUPABASE_PUBLISHABLE_KEY` no navegador. Configure os valores localmente em `.env` ou nas variáveis do provedor de deploy. Nunca publique chaves secretas ou `.env`.

## Instalação local

1. Instale Node.js e Bun (ou use npm se preferir).
2. Copie `.env.example` para `.env` e configure as variáveis do seu projeto.
3. Instale as dependências com `bun install` (o projeto inclui `bun.lock`) ou `npm install`.
4. Execute `bun run dev` para desenvolver e `bun run build` para verificar a compilação.

## Banco de dados

O projeto inclui migrações em `supabase/migrations/` e scripts de instalação completa em `SUPABASE_INSTALACAO/`. Os scripts numerados dessa última pasta destinam-se a uma instalação nova; não os execute em um banco já populado sem comparar o schema e revisar as migrações.

## Segurança

- `.env` e outros arquivos de ambiente ficam fora do Git.
- Use somente a chave publicável/anon no frontend.
- Nunca coloque `service_role` ou chaves `sb_secret_...` em código cliente, exemplos públicos ou commits.
- Mantenha RLS ativado e valide as políticas antes de conceder acesso à Data API.
