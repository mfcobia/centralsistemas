# Central de Sistemas · Meireles & Freitas

Site com os sistemas do time de Marketing · Produtos e Inovação, nas cores do guia de marca M&F 2024.

## A documentação fica no Manual (com senha)

Tudo sobre os sistemas está no **Manual da Central**, em `/central/manual/`: como cada sistema funciona, pendências, acessos, tarefas do dia a dia, os SQLs prontos para copiar e o código da sincronização.

- O conteúdo fica **criptografado** (AES-256) no arquivo `central/manual/dados.js`. Sem a senha, ninguém lê, mesmo olhando o código.
- A senha é passada pessoalmente pela gestão anterior. Não escreva a senha neste repositório.
- Para atualizar o Manual, use o botão **Editar** dentro dele, gere a nova versão e suba o `dados.js` novo em `central/manual/`.

## O que tem aqui

```
index.html     → abre a Central (/central/)
central/       → os sistemas (cada um é um único arquivo HTML) e o Manual
ferramentas/   → gerador de chave da sincronização (roda só no navegador)
```

## Regras de ouro

- **Este repositório é público.** Não suba senhas, tokens, a chave `service_role` do Supabase nem a chave da sincronização.
- As chaves `sb_publishable_...` e `anon` que aparecem nos HTML são públicas por natureza. A segurança vem das regras do banco.
- **Para mudar um sistema:** edite o HTML dele em `central/` e suba. Não há etapa de compilar.
