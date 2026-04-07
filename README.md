# Proposal Generator — Jonel Engenharia

Sistema para geracao de propostas tecnico-comerciais em HTML standalone, interativas e premium.

## Fluxo de uso

1. Copie `data/proposal-example.json` e preencha com os dados do novo cliente/projeto
2. Abra `prompts/master-prompt.md` e copie o prompt
3. Cole o prompt no Claude junto com o JSON preenchido
4. Claude gera o HTML final
5. Salve como `output/proposta-[cliente]-[data].html`
6. Abra no navegador, revise e envie ao cliente

## Estrutura

```
assets/          Logo e icones
data/            Schema e exemplos JSON
prompts/         Prompts para Claude
src/             Regras visuais de referencia
output/          HTMLs gerados
```

## Paleta visual

| Elemento          | Cor                      |
|-------------------|--------------------------|
| Fundo principal   | #F7F8FA                  |
| Fundo secundario  | #EEF1F5                  |
| Card              | #FFFFFF                  |
| Texto principal   | #111827                  |
| Texto secundario  | #4B5563                  |
| Vermelho marca    | #D63A34                  |
| Vermelho hover    | #B92E29                  |
| Dourado destaque  | #D6A645                  |
| Bordas            | #D7DCE3                  |

## Tipografia

Inter (fallback: system-ui, -apple-system, sans-serif)

## Campos obrigatorios no JSON

- `brand.companyName`
- `proposalMeta.proposalTitle`
- `client.clientName`
- `client.projectName`
- `proposalMeta.date`
- Pelo menos 1 item em `scopeItems`
- `pricing.total`
- `pricing.paymentTerms`
- `contact.company`
