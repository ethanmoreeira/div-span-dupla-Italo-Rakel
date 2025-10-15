# Relatório Final — Dupla Ítalo & Rakel

## O que aprendemos
- Diferença prática entre elementos block, inline e inline-block, com exemplos visuais.
- Aplicação do Box Model para evidenciar content/padding/border/margin no layout.
- Impacto de `display` nas propriedades `width`/`height` e em margens verticais.
- Importância de HTML/CSS semântico (lang, meta viewport, cabeçalho/rodapé, navegação).
- Fluxo de trabalho com LLMs: gerar, comparar, depurar e documentar.

## Diferenças entre LLMs
- LLM #1 (GPT-5): mais detalhado e didático; produziu estrutura com landmarks e comentários.
- LLM #2 (Perplexity): objetivo e ágil; exemplos curtos e visuais, exigindo menos leitura.

## Erros comuns e correções
- SPAN com `width/height` sem efeito em inline → solução: `display:inline-block`.
- Typo de CSS `font-wieght` → correção: `font-weight`.
- Seletor não batendo no alvo (`div.cartao-primario` vs `article.cartao-primario`).
- Margens verticais em inline não empurram layout → usar `inline-block` ou `block`.

## Prints/links
- Base: `01-base/index.html`
- Experimentos: `02-experimentos/inline-para-block.html`, `02-experimentos/inline-block.html`, `02-experimentos/comparativo.html`
- Bugs e Correções: `03-bugs-e-correcoes/codigo-com-bugs.html`, `03-bugs-e-correcoes/correcoes.html`

---

Autores: Ítalo (LLM #1 — GPT-5) e Rakel (LLM #2 — Perplexity)
