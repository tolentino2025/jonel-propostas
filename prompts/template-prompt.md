# Prompt Complementar — Modo Template Reutilizavel

Use este prompt APOS gerar a primeira versao, para transformar o HTML em template base.

---

## PROMPT

```
Quero que voce trate este projeto como um template base reutilizavel para geracao de propostas tecnico-comerciais em HTML.

Regras:
- Nao criar uma proposta unica e engessada
- Criar uma arquitetura de template reutilizavel
- Separar claramente:
  1. Dados (objeto JSON)
  2. Layout (estrutura HTML)
  3. Componentes (blocos visuais)
  4. Interacoes (JS)
- O HTML deve aceitar variacoes de:
  - Quantidade de itens de escopo (1 a N)
  - Opcionais (0 a N)
  - Exclusoes (0 a N)
  - Valores
  - Cliente
  - Projeto
  - Prazo
  - CTA
- Crie componentes reutilizaveis para:
  - Hero slide (capa)
  - Sumario navegavel
  - Cards de escopo com accordion
  - Timeline horizontal
  - Pricing cards
  - Highlights/diferenciais
  - CTA section
  - Rodape de contato
- O codigo deve ser facil de adaptar
- Use nomenclatura clara de classes e funcoes
- Adicione comentarios estruturais no codigo
- Pense como um design system de propostas
- Inclua no topo do HTML um bloco <script> com o objeto PROPOSAL_DATA
  que alimenta todos os componentes dinamicamente
- Ao trocar apenas o objeto PROPOSAL_DATA, a proposta inteira se atualiza

Paleta:
- Fundo principal: #F7F8FA
- Fundo secundario: #EEF1F5
- Card: #FFFFFF
- Texto principal: #111827
- Texto secundario: #4B5563
- Vermelho marca: #D63A34
- Vermelho hover: #B92E29
- Dourado destaque: #D6A645
- Bordas: #D7DCE3
```
