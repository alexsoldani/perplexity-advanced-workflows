# Perplexity Advanced Workflows

> Documentação completa, análise profunda e workflows avançados baseados no system prompt oficial do Perplexity AI.

Este repositório foi criado para quem quer **extrair o máximo** do Perplexity, entendendo como ele realmente funciona por dentro e criando workflows profissionais e reproduzíveis.

---

## 📚 O que você vai encontrar aqui

- **Análise profunda** do system prompt oficial do Perplexity
- **Padrões de workflow** testados e documentados
- **Templates prontos** para diferentes tipos de uso (pesquisa acadêmica, notícias, código, etc.)
- **Best practices** extraídas diretamente do comportamento real do Perplexity
- **Versões melhoradas** do prompt original

---

## 🗂️ Estrutura do Repositório

```
perplexity-advanced-workflows/
├── README.md
├── docs/
│   ├── analysis/
│   │   └── deep-analysis-perplexity-prompt.md
│   └── best-practices.md
└── workflow-patterns.md
├── templates/
│   ├── academic-research.md
│   ├── news-summarization.md
│   ├── technical-deep-dive.md
│   ├── cooking-recipe.md
│   └── custom-workflow-template.md
├── prompts/
│   └── enhanced-perplexity-prompt.md
└── examples/
    └── (exemplos reais de uso)
```

---

## 🔍 Análise do System Prompt Original

O arquivo original (`Perplexity/Prompt.txt`) foi extraído do repositório [system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools).

Fizemos uma análise detalhada que revela:

- A arquitetura de **dois sistemas** (planejamento + síntese)
- O rigoroso sistema de **citações inline**
- As regras extremamente detalhadas de **formatação**
- O roteamento por **tipo de query**
- As restrições de segurança e qualidade

→ Leia a análise completa: [docs/analysis/deep-analysis-perplexity-prompt.md](./docs/analysis/deep-analysis-perplexity-prompt.md)

---

## 🚀 Workflows Recomendados

### 1. Pesquisa Acadêmica / Técnica
- Use o template `academic-research.md`
- Peça respostas longas e estruturadas com seções
- Sempre exija citações logo após cada afirmação relevante

### 2. Resumo de Notícias e Atualizações
- Use o template `news-summarization.md`
- Peça agrupamento por tópicos + fontes diversas
- Priorize fontes confiáveis

### 3. Deep Dive Técnico / Código
- Use o template `technical-deep-dive.md`
- Peça primeiro o código em bloco, depois a explicação
- Use para arquitetura, debugging e decisões técnicas

### 4. Receitas e Instruções Passo a Passo
- Use o template `cooking-recipe.md`
- Exija ingredientes com quantidades + instruções numeradas

### 5. Workflow Personalizado
- Use o `custom-workflow-template.md` como base
- Adapte as regras de formatação e tipo de resposta

---

## 📌 Best Practices Extraídas

Baseado na análise do prompt oficial:

- **Nunca comece a resposta com cabeçalho** (`##`). Sempre inicie com 2-4 frases de resumo.
- **Use tabelas** para comparações em vez de listas longas.
- **Cite fontes inline** usando o formato `[1]` imediatamente após a frase.
- **Evite emojis**, hedging e linguagem moralizadora.
- **Adapte o estilo** conforme o tipo de query (acadêmico, notícia, código, etc.).
- **Mantenha o tom jornalístico** e de especialista.

---

## 🛠️ Como Usar Este Repositório

1. Clone o repositório
2. Leia a análise profunda primeiro
3. Escolha o template mais adequado ao seu caso de uso
4. Copie o template para o Perplexity (ou use como base para criar prompts customizados)
5. Adapte conforme sua necessidade

---

## 🤝 Contribuições

Este repositório foi criado com base em engenharia reversa de prompts reais. Contribuições são bem-vindas, especialmente:

- Novos workflows testados
- Melhorias nos templates
- Análises de novos prompts do Perplexity (caso sejam atualizados)

---

## 📄 Licença

Este projeto está sob licença MIT. Sinta-se livre para usar, modificar e compartilhar.

---

**Criado em Junho de 2026** com base no system prompt extraído do repositório de prompts de ferramentas de IA.