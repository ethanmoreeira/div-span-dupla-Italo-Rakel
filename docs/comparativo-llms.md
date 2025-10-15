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

| Critério | GPT-5 (Pessoa A) | Perplexity (Pessoa B) |
|:--|:--|:--|
| *1. Clareza nas explicações* | Explicações técnicas e bem estruturadas, com termos precisos e exemplos diretos. | Explicações mais curtas e objetivas, com foco prático e menos terminologia técnica. |
| *2. Qualidade do código HTML/CSS* | Código limpo, indentação consistente e comentários didáticos; usou landmarks semânticos. | Código funcional e conciso, com exemplos bem separados e boas práticas mantidas. |
| *3. Correção técnica (semântica e sintaxe)* | 100% válido em HTML5 e CSS3; uso correto de propriedades. | 99% correto; pequeno risco de variação estética, mas sem erros estruturais. |
| *4. Didática (clareza visual e pedagógica)* | Fortemente didático, com cores e comentários guiando o leitor. | Visual mais simples e direto; ótimo para demonstração objetiva. |
| *5. Uso de boas práticas e acessibilidade* | Usou landmarks (header, main, footer), aria-label e ícones com aria-hidden="true". | Manteve estrutura semântica, mas reduziu metadados de acessibilidade. |
| *6. Originalidade nas respostas* | Ofereceu justificativas detalhadas e contextualização teórica. | Focou em exemplos e experimentos práticos (inline→block, inline-block). |
| *7. Capacidade de depuração e adaptação* | Explicou como cada camada do Box Model afeta o layout. | Destacou as diferenças de comportamento entre SPAN e DIV em execução. |

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