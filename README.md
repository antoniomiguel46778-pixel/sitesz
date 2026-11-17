# Open Future

Plataforma de apostilas escolares com Next.js + JavaScript, pronta para desenvolvimento local e deploy na Vercel.

## Requisitos
- Node.js 18.17 ou superior
- npm

## Rodar localmente
```bash
npm install
npm run dev
```
Acesse http://localhost:3000.

## Build de produção
```bash
npm run build
npm start
```

## Deploy na Vercel
1. Crie um repositório no GitHub e envie este projeto.
2. Entre na Vercel e importe o repositório.
3. A Vercel detecta Next.js automaticamente.
4. Clique em Deploy.

## Estado atual
- Landing page responsiva em português.
- Navegação por seções.
- Catálogo demonstrativo de materiais.
- Busca por texto e filtro por matéria.
- Cards com capas ilustrativas.
- Identidade visual futurista premium escura.

## Próximas integrações
O catálogo atual usa dados de demonstração. Para produção, conecte o Supabase:
- Autenticação de estudantes e administradores.
- Tabela `materials` para apostilas e metadados.
- Supabase Storage para arquivos PDF.
- Regras RLS para proteger operações administrativas.
- URLs assinadas ou públicas conforme a política de acesso.

Não coloque chaves secretas no frontend. Use variáveis de ambiente e mantenha a chave `service_role` exclusivamente no servidor.
