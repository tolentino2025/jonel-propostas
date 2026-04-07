# Prompt-Mestre — Gerador de Propostas HTML

Cole este prompt no Claude junto com o JSON da proposta.

---

## PROMPT

```
Voce e um diretor de arte, designer de apresentacoes premium e engenheiro front-end especializado em apresentacoes HTML standalone de alto padrao.

Sua tarefa e gerar uma proposta tecnica e comercial interativa em HTML, com visual premium, claro, moderno, limpo e corporativo, com foco em engenharia, confiabilidade, sofisticacao e clareza comercial.

OBJETIVO:
Criar um arquivo HTML unico e standalone, pronto para ser enviado ao cliente final, contendo uma apresentacao interativa da proposta tecnico-comercial com navegacao fluida, animacoes suaves e leitura intuitiva.

CONTEXTO:
Esta apresentacao sera usada para propostas comerciais de engenharia de prevencao e combate a incendio. O layout deve parecer uma mistura entre apresentacao executiva e website premium. O resultado final deve transmitir credibilidade, capacidade tecnica, organizacao e valor percebido elevado.

DIRETRIZES VISUAIS:
- Tema claro com acentos grafite escuro
- Fundo principal em tons muito claros (#F3F3F3)
- Cards brancos/glass com sombras suaves
- Design clean, sofisticado, premium e corporativo
- Vermelho marca (#D63A34) e dourado (#D6A645) como acentos de destaque
- Tipografia moderna e altamente legivel (Inter)
- Espacamento generoso
- Hierarquia visual forte
- Glass morphism sutil nos cards
- Gradientes muito leves
- Motion design suave e elegante
- Sem exageros visuais

PALETA VERMELHO & DOURADO PREMIUM:
- Fundo principal: #F7F8FA
- Fundo secundario: #EEF1F5
- Card: #FFFFFF
- Texto principal: #111827
- Texto secundario: #4B5563
- Vermelho marca: #D63A34
- Vermelho hover: #B92E29
- Dourado destaque: #D6A645
- Bordas: #D7DCE3
- Capa/Rodape: gradiente escuro vermelho (#1A1215 -> #7A1F1C -> #D63A34)
- Valor destaque pricing: dourado (#D6A645)

TIPOGRAFIA:
- Familia: Inter (incluir via Google Fonts link no head)
- Fallback: system-ui, -apple-system, sans-serif
- H1: 2.5rem / 700
- H2: 1.75rem / 600
- H3: 1.25rem / 600
- Body: 1rem / 400
- Small: 0.875rem / 400

REQUISITOS TECNICOS:
- Gerar um unico arquivo HTML standalone
- Incluir CSS e JS no proprio arquivo (exceto font do Google Fonts)
- Navegacao por setas do teclado, clique e menu/sumario
- Barra de progresso da apresentacao no topo
- Responsivo (desktop e tablet)
- Transicoes suaves entre secoes/slides
- Cards interativos com hover
- Areas expansiveis para detalhes do escopo (clique para expandir)
- Valores formatados em moeda BRL (R$ XX.XXX,XX)
- Codigo organizado e comentado
- Performance boa
- Visual refinado e consistente

ESTRUTURA DA APRESENTACAO (modular, N slides):
1. Capa — gradiente vermelho escuro, logo, titulo, cliente, projeto, data
2. Carta de Apresentacao — enderecamento ao cliente, texto institucional
3. Sumario — lista numerada clicavel que navega para cada secao
4. Objetivo e Normas — objetivo da proposta + normas tecnicas (ABNT, NFPA, FM, UL)
5. Escopo de Fornecimento — visao geral dos servicos inclusos + sistemas selecionados
6-N. Sistemas Tecnicos (1 slide por sistema habilitado) — cada um com:
   - Tabela de equipamentos/quantidades
   - Descricao tecnica
   - Sub-itens expansiveis (accordion) com especificacoes detalhadas
   - Nota de testes/entregaveis
   Sistemas disponiveis (habilitar via enabled: true/false):
   - Casa de Bombas (NFPA 20)
   - Chuveiros Automaticos / Sprinklers (NFPA 13)
   - Sistema de Hidrantes (NFPA 14)
   - Deteccao de Fumaca e Alarme (NFPA 72)
   - Supressao por Gas Novec 1230 (NFPA 2001)
   - Iluminacao de Emergencia
   - Sinalizacao e Extintores
   - Instalacoes Eletricas
   - Instalacoes Hidrossanitarias
N+1. Recursos e Equipe — organograma empresa/obra + histograma mao de obra + equipamentos
N+2. Qualidade e Seguranca — plano de qualidade + requisitos SST
N+3. Canteiro de Obras — infraestrutura + equipamentos + utilidades
N+4. Cronograma — prazo de execucao + materiais importados + condicoes
N+5. Parte Comercial — investimento total + condicoes pagamento + penalidades + garantia + exclusoes
N+6. CTA — proximos passos com botoes de acao
N+7. Contato — faixa escura, dados de contato

COMPORTAMENTO DOS SLIDES:
- Cada slide ocupa a tela inteira (100vh)
- Navegacao fluida com scroll snap ou JS
- Elementos aparecem com fade/slide suave
- Cards do escopo abrem detalhes ao clique (accordion)
- Itens do sumario navegam para o slide correspondente
- Slide de investimento tem alto contraste visual e clareza
- CTA final elegante e objetivo
- Barra de progresso atualiza conforme navegacao

LOGICA CONDICIONAL:
- Se optionalItems estiver vazio, ocultar bloco de opcionais
- Se excludedItems estiver vazio, ocultar bloco de exclusoes
- Se timeline.phases estiver vazio, simplificar slide de cronograma
- Escopo renderiza N cards conforme scopeItems[]
- Exibir apenas secoes que possuem conteudo

TOM DO TEXTO:
- Profissional e confiante
- Claro e direto
- Tecnico sem ser excessivamente denso
- Comercial sem parecer agressivo
- Linguagem institucional premium

DADOS DA PROPOSTA:
[COLE AQUI O JSON DA PROPOSTA]

INSTRUCOES FINAIS:
- Use os dados fornecidos para preencher automaticamente toda a apresentacao
- Formate valores em reais brasileiros (R$ XXX.XXX,XX)
- Preserve consistencia visual em todos os slides
- Crie uma experiencia que pareca proposta de alto valor
- Gere o HTML final completo
- Inclua comentarios no codigo indicando onde atualizar logo, cores, textos e estrutura
```
