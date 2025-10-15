# Comparativo entre LLMs — GPT-5 × Perplexity

*Dupla:* Ítalo & Rakel  
*Branchs:*  
- Ítalo → main (LLM #1: GPT-5)  
- Rakel → rakel-llm2 (LLM #2: Perplexity)  

*Objetivo:*  
Comparar o desempenho, clareza e consistência das duas LLMs utilizadas no desenvolvimento do projeto *DIV × SPAN — Block-Level vs Inline-Level*, avaliando a produção de código, explicações e capacidade de depuração.

---

## 1. Contexto do Experimento

Durante o trabalho, cada integrante utilizou uma LLM diferente para gerar, explicar e revisar exemplos práticos em HTML e CSS:

| Pessoa | LLM utilizada | Versão | Função principal |
|:--|:--|:--|:--|
| Ítalo | GPT-5 | OpenAI | Geração inicial e estrutura base (Prompts 1–3) |
| Rakel | Perplexity | Modelo LLM #2 | Revisão, complementos e novos experimentos (Prompts 4–6) |

As duas versões trabalharam sobre o mesmo tema:  
> “Diferença entre elementos *block-level* e *inline-level* e uso de DIV e SPAN no layout.”

---

## 2. Critérios de Avaliação

# Tabela de notas (0–5)

| Critério (0–5) | LLM #1 — GPT-5 (Ítalo) | LLM #2 — Perplexity (Rakel) | Observações |
|:--|:--:|:--:|:--|
| Correção técnica (block/inline/inline-block) | 5 | 4 | GPT-5 manteve semântica e sintaxe impecáveis; Perplexity correto, com poucos detalhes omitidos |
| HTML/CSS semântico e limpo | 5 | 4 | Estrutura com landmarks e navegação; LLM #2 direto e funcional |
| Depuração (bugs encontrados e fixados) | 5 | 4 | Diagnóstico e correção claros; LLM #2 acertou soluções com menos explicação |
| Clareza das explicações | 5 | 4 | LLM #1 mais didático; LLM #2 mais objetivo |
| Acessibilidade mínima | 4 | 3 | Uso de lang e landmarks; ainda há espaço para rótulos/aria em exemplos |
| **Média** | **4.8** | **3.8** |  |

# Comparativo de LLMs (GPT-5 vs Perplexity)

| Critério      | GPT-4 (Ítalo)                                       | Perplexity (Rakel)                                      |
|---------------|-----------------------------------------------------|---------------------------------------------------------|
| **Clareza**   | Respostas mais detalhadas e coesas, facilitando a compreensão geral. | Respostas em formato de pontos; claras, mas menos elaboradas que o GPT-4. |
| **Corretude** | Geralmente muito preciso e consistente com conceitos técnicos (ex.: Box Model). | Preciso nas explicações básicas; em alguns casos faltou detalhamento na sintaxe. |
| **Utilidade** | Forneceu explicações aprofundadas e exemplos completos, úteis para aprendizado. | Útil para gerar estrutura inicial; exigiu revisão adicional para detalhes. |
| **Criatividade** | Introduziu explicações originais e exemplos variados além do óbvio. | Criativo nos exemplos visuais, mas seguiu respostas mais objetivas. |


---

## 3. Resultados Gerais

| Aspecto | Melhor desempenho | Observações |
|:--|:--|:--|
| *Clareza conceitual* | GPT-5 | Maior aprofundamento teórico. |
| *Objetividade e foco prático* | Perplexity | Mostrou rapidamente o efeito visual esperado. |
| *Didática visual* | Empate | Ambos foram claros, mas em estilos diferentes. |
| *Correção técnica e estrutura* | GPT-5 | Estrutura mais detalhada, com landmarks e comentários extensos. |
| *Inovação nas respostas* | Perplexity | Trouxe variações interessantes no uso de display:inline-block e flexbox. |

---

## 4. Análise descritiva

Durante a comparação prática:
- O *GPT-5* demonstrou excelente domínio técnico e semântico, produzindo um código mais próximo do que o professor espera em um *ambiente educacional estruturado*.  
- O *Perplexity, por outro lado, se destacou na **rapidez* e na *objetividade, entregando exemplos funcionais e curtos, ideais para **testes de comportamento*.

A união dos dois gerou um resultado equilibrado:
- A base conceitual do GPT-5 garantiu robustez;  
- Os exemplos de Perplexity tornaram o aprendizado mais visual e direto.

---

## 5. Conclusão Geral

*Conclusão:*  
Ambas as LLMs foram eficazes no desenvolvimento do projeto.  
O GPT-5 se sobressaiu em clareza teórica e padronização semântica,  
enquanto o Perplexity demonstrou agilidade e foco prático na aplicação visual.

A integração das duas abordagens resultou em um material *completo, didático e tecnicamente sólido*, atingindo plenamente os objetivos do professor:
> diferenciar e demonstrar, de forma funcional, os comportamentos de elementos block, inline e inline-block, com documentação e revisão feitas por duas inteligências artificiais distintas.

---

*Autores:*  
- Ítalo — GPT-5 (LLM #1)  
- Rakel — Perplexity (LLM #2)  
*Entrega:* Passo 2 — Comparativo entre LLMs  
*Status:* ✅ Concluído e validado