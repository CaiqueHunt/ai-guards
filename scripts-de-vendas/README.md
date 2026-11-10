# Scripts de Vendas e Apresentações

Pasta central para criação de roteiros (scripts) de venda e decks de apresentação.

## Estrutura

```
scripts-de-vendas/
├── README.md                      # Este arquivo
├── guias/                         # Método e padrões válidos para qualquer variação
│   ├── guia-estrutura-roteiro.md  # Sequência-base do roteiro de venda
│   └── guia-apresentacao.md       # Como montar o deck a partir do roteiro
└── variacoes/                     # Uma pasta por produto / público / contexto
    └── investimento-imoveis-eua/  # Variação: cotas de investimento imobiliário nos EUA
        ├── rascunho-roteiro/      # Rascunhos e argumentos do roteiro desta variação
        │   ├── roteiro-rascunho.md
        │   └── argumentos-linha-a-linha.md
        └── transcricoes/          # Transcrições das reuniões que originaram o roteiro
            └── 2026-11-03-reuniao-caique-igor.md
```

## Como criar uma nova variação

1. Crie `variacoes/<nome-da-variacao>/` com as subpastas `rascunho-roteiro/` e `transcricoes/`.
2. Salve as transcrições de reuniões em `transcricoes/`, nomeadas por data (`AAAA-MM-DD-descricao.md`).
3. Extraia os argumentos das transcrições para `rascunho-roteiro/argumentos-linha-a-linha.md`, com timestamp.
4. Monte o `roteiro-rascunho.md` seguindo a sequência de `guias/guia-estrutura-roteiro.md`.
5. Quando o roteiro estiver validado, derive o deck seguindo `guias/guia-apresentacao.md`.

## Convenções

- Idioma: português.
- Nomes de pastas e arquivos em minúsculas, sem acento, separados por hífen.
- Toda fala extraída de transcrição deve citar o timestamp de origem.
- Transcrições automáticas podem conter erros; registre as correções conhecidas no topo do arquivo.
