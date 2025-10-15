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

# Prompt Log — Passo 2 (Pessoa B — Rakel, LLM #2: Perplexity)

*Responsável:* Rakel  
*LLM usada:* Perplexity (LLM #2)  
*Branch:* rakel-llm2   

---

## Objetivo do Passo 2
Aplicar novamente os Prompts 1 a 6 utilizando uma segunda LLM (Perplexity), com foco em:
- Reforçar o entendimento prático entre elementos *block-level* e *inline-level*;  
- Criar exemplos funcionais em HTML/CSS (DIV, SPAN, inline-block);  
- Documentar respostas e decisões da IA durante a geração e revisão dos códigos;  
- Demonstrar independência na construção dos exemplos e consistência com a versão da Pessoa A (GPT-5).

---

## Prompt 1 — Definição curta (Block vs Inline)

*Prompt:*  
> Explique, em até 4 linhas, a diferença entre elementos block-level e inline-level, com 2 exemplos reais de cada e quando usar DIV e SPAN.

*Resposta da LLM (resumo):*  
- Elementos *block-level* ocupam toda a largura disponível e quebram linha automaticamente (<div>, <p>).  
- Elementos *inline* ocupam apenas o espaço necessário, permanecendo na mesma linha (<span>, <a>).  
- Regra prática: usar <div> para estruturar blocos e <span> para destacar trechos dentro de um texto.

*Aplicação:*  
Adicionado parágrafo explicativo sob o <h1> no 01-base/index.html.

*Commit:*  
feat(llm2): Prompt 1 — definição curta block × inline (Perplexity)

---

## Prompt 2 — MVP Base (DIV x SPAN)

*Prompt:*  
> Gere uma página mínima “DIV × SPAN” com 3 cartões organizados com DIV (block) e textos/ícones com SPAN (inline). Use CSS externo, HTML semântico e landmarks.

*Resposta da LLM (resumo):*  
A IA gerou uma página com três *cartões (DIV), cada um contendo ícones e textos em **SPAN*, com estrutura semântica (header, main, footer), navegação e CSS externo para organização visual.

*Aplicação:*  
- Arquivo: 01-base/index.html  
- CSS: 01-base/styles.css  
- Layout flexível, bordas suaves e ícones inline.  

*Decisão:*  
Padronizar nomes de arquivos (em inglês), manter styles.css e preservar cores neutras e estrutura responsiva.  

*Commit:*  
feat(llm2): Prompt 2 — base DIV x SPAN com layout e semântica

---

## Prompt 3 — Box Model Visível

*Prompt:*  
> Aplique padding, border, margin e outline nos cartões para evidenciar as camadas do Box Model. Explique em 2–3 linhas como cada camada afeta o layout.

*Resposta da LLM (resumo):*  
- *Content:* espaço real do conteúdo.  
- *Padding:* espaçamento interno entre conteúdo e borda.  
- *Border:* linha ao redor do elemento.  
- *Margin:* espaçamento externo entre elementos.  
- *Outline:* destaque visual sem afetar o fluxo.  

*Aplicação:*  
- Atualizado 01-base/styles.css (padding: 20px; border: 6px solid; margin: 16px; outline tracejado).  
- Adicionado texto explicativo “Box Model (visível)” abaixo dos cartões no index.html.  

*Commit:*  
feat(llm2): Prompt 3 — Box Model visível (content/padding/border/margin + explicação)

---

## Prompt 4 — Inline → Block

*Prompt:*  
> Demonstre a conversão de <span> de inline para display:block, com comparação antes/depois e texto explicativo.

*Resposta da LLM (resumo):*  
O Perplexity gerou exemplo com dois estados:  
- *Antes:* <span> inline, fluindo no texto.  
- *Depois:* <span> com display:block, quebrando linha e ocupando toda a largura.  

*Aplicação:*  
Arquivo: 02-experimentos/inline-para-block.html  
Inclui: cabeçalho explicativo, navegação entre páginas e comparação visual “Antes e Depois”.

*Commit:*  
feat(llm2): Prompt 4 — inline→block (comparativo antes/depois)

---

## Prompt 5 — Inline-block

*Prompt:*  
> Demonstre display:inline-block, mostrando elementos lado a lado que aceitam largura e altura, comparando com inline padrão.

*Resposta da LLM (resumo):*  
Criado exemplo com SPANs padrão (inline) e SPANs modificados para inline-block, com dimensões fixas (width:200px; height:60px;), texto centralizado e layout horizontal.

*Aplicação:*  
Arquivo: 02-experimentos/inline-block.html  
Duas seções: “Inline padrão” e “Inline-block”, exibindo o contraste visual.

*Commit:*  
feat(llm2): Prompt 5 — demonstração inline-block (lados a lado com dimensões fixas)

---

## Prompt 6 — Comparativo Final

*Prompt:*  
> Crie um comparativo visual entre elementos block-level (DIV), inline-level (SPAN) e inline-block, organizados lado a lado com legendas explicativas.

*Resposta da LLM (resumo):*  
Página com *duas colunas* (usando flexbox):  
- Coluna esquerda: três DIVs empilhadas (block).  
- Coluna direita: quatro SPANs inline (lado a lado).  
Legenda final explica a diferença visual e estrutural.

*Aplicação:*  
Arquivo: 02-experimentos/comparativo.html  
Inclui: título centralizado, legendas, bordas coloridas e navegação para as demais páginas.

*Commit:*  
feat(llm2): Prompt 6 — comparativo visual DIV × SPAN × inline-block

---

## Conclusão do Passo 2 (Pessoa B — Rakel)

*Resultados alcançados:*
- Estrutura completa replicada com Perplexity (LLM #2);  
- Páginas HTML e CSS revisadas com consistência visual e semântica;  
- Box Model aplicado corretamente;  
- Três experimentos distintos demonstrando display inline, block e inline-block;  
- Navegação entre páginas e comentários didáticos inclusos;  
- Documentação completa dos Prompts 1–6 no prompt-log.md.  

 
*Responsável:* Rakel  
*Branch:* rakel-llm2  
*Status:* ✅ Passo 2 concluído e validado.

---
