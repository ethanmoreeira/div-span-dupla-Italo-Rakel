## 2025-10-08 — Passo 1–2 (Preparação)

**Responsável:** Ítalo (Pessoa A)  
**LLM usada:** — (fase sem LLM)  

**Resumo:**  
Criação da estrutura completa do repositório (`01-base`, `02-experimentos`, `03-bugs-e-correcoes`, `docs`),  
incluindo o arquivo `README.md`, configuração do Git e publicação no GitHub.  
Implementação da base (`index.html` + `styles.css`) e dos 3 experimentos:  
- `inline-para-block.html` (conversão de inline para block)  
- `inline-block.html` (demonstração de inline-block)  
- `comparativo.html` (comparativo lado a lado entre DIV x SPAN)  

**Decisões:**  
- Usar bordas e cores para evidenciar o Box Model.  
- Inserir comentários didáticos em todo o HTML/CSS.  
- Criar navegação entre as páginas para facilitar a verificação no navegador.  
- Deixar o arquivo `codigo-com-bugs.html` preparado para a fase da Parceira (Pessoa B).

---
## 2025-10-08 — Passo 1 (Geração Base com LLM #1)

**Responsável:** Ítalo (Pessoa A)  
**LLM usada:** GPT-5 (LLM #1)  

**Prompt 1 – Definição curta:**  
Explique, em até 4 linhas, a diferença entre elementos block-level e inline-level, com 2 exemplos reais de cada.  

**Resposta (LLM #1):**  
Elementos block-level (ex.: `<div>`, `<p>`) ocupam toda a largura e iniciam nova linha.  
Elementos inline (ex.: `<span>`, `<a>`) permanecem no fluxo do texto, sem quebrar linha.  
Usa-se `DIV` para organizar blocos de layout e `SPAN` para destacar trechos no meio do texto.

---

**Prompt 2 – MVP (base):**  
Gere uma página mínima sobre “DIV × SPAN”: 3 cartões organizados com DIV (block) e textos/ícones com SPAN (inline). Sem frameworks.

**Resumo da Resposta (LLM #1):**  
A LLM gerou `index.html` com 3 DIVs e SPANS internos, comentários didáticos e CSS externo (`styles.css`).  
O código foi revisado por Ítalo e ajustado para cores educacionais e legibilidade.

---

**Prompt 3 – Box Model visível:**  
Ajuste o CSS para evidenciar content/padding/border/margin com cores e bordas.  
Explique em 3 linhas como cada camada afeta o layout.

**Resumo da Resposta (LLM #1):**  
A LLM adicionou cores e bordas visuais no `styles.css`, tornando o Box Model visível.  
Ítalo testou no navegador e confirmou que as camadas (content, padding, border, margin) ficaram claras.
