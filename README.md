# Agenda — Vitor Car Auto Center

Aplicação de agenda para oficina mecânica com React, TypeScript, Vite e Supabase.

## Executar localmente
1. Instale Node.js LTS.
2. No terminal, dentro da pasta do projeto: `npm install`
3. Copie `.env.example` para `.env.local` e preencha `VITE_SUPABASE_URL` e `VITE_SUPABASE_ANON_KEY` com os dados do projeto Supabase.
4. No SQL Editor do Supabase, execute `supabase/schema.sql`.
5. Execute `npm run dev` e abra o endereço local exibido.

Sem credenciais do Supabase, a tela funciona em modo de demonstração; os dados não são persistidos.

## Segurança antes de produção
O SQL fornecido contém políticas abertas para facilitar um protótipo. Antes de usar com dados reais, configure autenticação e substitua essas políticas por regras restritas a usuários autorizados. Nunca coloque a `service_role key` no frontend.
