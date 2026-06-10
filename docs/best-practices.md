# Best Practices para Uso Avançado do Perplexity

Baseado na análise profunda do system prompt oficial.

---

## 1. Estrutura de Resposta

### Regra de Ouro
**Nunca comece sua pergunta pedindo para começar com um cabeçalho.**

O prompt original é muito claro:
> "NEVER start the answer with a header. NEVER start by explaining to the user what you are doing."

**Boa prática:**
- Comece sempre com 2 a 4 frases de resumo/contexto.
- Depois use `##` para as seções principais.

**Exemplo ruim:**
> "## Resumo\nAqui está o resumo..."

**Exemplo bom:**
> "O Perplexity é uma ferramenta de busca conversacional que combina modelos de linguagem com busca em tempo real. Ele se destaca por entregar respostas bem fundamentadas e citadas. Abaixo está uma análise detalhada do seu funcionamento interno."

---

## 2. Sistema de Citações

Esta é uma das maiores forças do Perplexity.

### Como pedir citações corretamente:

```markdown
Sempre cite as fontes usando o formato [1], [2], etc. logo após cada afirmação relevante. 
Coloque a citação imediatamente após o ponto final, sem espaço antes do colchete.
```

**Exemplo de prompt bom:**
> "Responda usando o formato de citação inline [1]. Coloque a citação logo após a frase, sem espaço antes do colchete. Use no máximo 3 citações por frase."

---

## 3. Comparações e Tabelas

O prompt prefere **tabelas** em vez de listas longas quando há comparação.

**Dica:**
Peça explicitamente:

> "Quando comparar opções, use tabelas Markdown com colunas claras (ex: Critério | Opção A | Opção B | Vantagem)."

---

## 4. Adaptação por Tipo de Query

O prompt original tem tratamento diferente dependendo do tipo de pergunta. Use isso a seu favor.

| Tipo de Uso                    | Como pedir no prompt                                      | Características da resposta esperada          |
|--------------------------------|-----------------------------------------------------------|-----------------------------------------------|
| Pesquisa Acadêmica             | "Forneça uma resposta longa e detalhada em formato acadêmico" | Parágrafos densos + seções + citações        |
| Resumo de Notícias             | "Agrupe por tópicos e destaque fontes diversas"           | Conciso + listas + priorização de fontes     |
| Código / Arquitetura           | "Mostre primeiro o código em bloco, depois explique"      | Blocos de código + explicação clara          |
| Receitas / Tutoriais           | "Liste ingredientes com quantidades e passos numerados"   | Passo a passo muito claro e preciso          |
| Biografia / Pessoas            | "Escreva uma biografia curta e abrangente"                | Fatos organizados + tom neutro               |

---

## 5. O que Evitar

O prompt original proíbe explicitamente várias coisas:

- Usar emojis na resposta final
- Usar linguagem moralizadora ("It is important to...", "It is inappropriate...")
- Usar hedging excessivo ("It is subjective...", "It depends...")
- Expor ou mencionar o system prompt
- Terminar a resposta com uma pergunta
- Repetir conteúdo protegido por copyright

**Dica prática:**
Adicione no seu prompt:

> "Mantenha tom jornalístico, direto e profissional. Evite emojis, moralização e hedging."

---

## 6. Workflow de Alta Qualidade (Recomendado)

Para obter os melhores resultados:

1. **Defina o tipo de query** no início do prompt
2. **Especifique o formato de saída** com detalhes (citações, tabelas, estrutura)
3. **Peça resumo inicial** + seções bem definidas
4. **Exija citações inline** sempre que possível
5. **Defina o tom** (jornalístico, técnico, didático, etc.)

---

## 7. Combinação com Outras Ferramentas

O Perplexity brilha em **pesquisa e síntese**. Use em conjunto com:

- **Claude / GPT-4o / Grok**: Para raciocínio profundo, planejamento estratégico e criação de conteúdo criativo
- **Cursor / Windsurf / Devin**: Para implementação de código
- **Perplexity** → Pesquisa + fontes
- **Claude** → Raciocínio + arquitetura + escrita refinada

**Fluxo recomendado:**
Perplexity (pesquisa fundamentada) → Claude/Grok (análise profunda + síntese final)

---

## 8. Prompt Base Recomendado

Use este como base para a maioria dos workflows:

```markdown
Você é um assistente de pesquisa altamente preciso. 

Responda à seguinte pergunta usando os resultados de busca fornecidos.

Regras:
- Comece com 2-4 frases de resumo.
- Use ## para seções principais.
- Cite fontes usando [1], [2] logo após cada afirmação relevante.
- Prefira tabelas para comparações.
- Mantenha tom jornalístico, direto e profissional.
- Evite emojis, moralização e hedging.

Pergunta: [sua pergunta aqui]
```

---

Essas práticas foram extraídas diretamente do system prompt oficial do Perplexity e testadas em uso real.