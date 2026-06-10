# Exemplo Real de Workflow: Tomada de Decisão Técnica (Arquitetura)

**Objetivo:** Tomar uma decisão técnica importante com boa análise de trade-offs.

---

## Workflow Completo

### Etapa 1: Definição do Problema e Critérios

**Prompt usado:**

```markdown
Preciso tomar uma decisão técnica importante:

Contexto: [DESCREVA O CONTEXTO]
Opções em consideração: [Liste as opções]
Critérios importantes para mim: [Liste os critérios, ex: performance, custo, complexidade, time-to-market, escalabilidade, etc.]

Primeiro, me ajude a refinar os critérios e identificar se tem algum critério importante que eu possa estar esquecendo.
```

### Etapa 2: Análise Comparativa (usando template Technical Deep Dive)

**Prompt usado:**

```markdown
[COLE AQUI O TEMPLATE DE TECHNICAL DEEP DIVE]

Analise os trade-offs entre as seguintes opções: [Opção A] vs [Opção B] vs [Opção C]

Crie uma tabela comparando os critérios que definimos anteriormente.
Para cada opção, liste os principais riscos e pontos de atenção.
```

### Etapa 3: Recomendação com Justificativa

**Prompt usado:**

```markdown
Com base na análise comparativa anterior, faça uma recomendação clara respondendo:

1. Qual opção você recomenda como principal?
2. Em quais cenários a segunda opção seria melhor?
3. Quais são os 3 maiores riscos da opção recomendada e como mitigar?
4. Quais seriam os próximos passos concretos para implementar a decisão?
```

### Etapa 4: Plano de Validação (opcional)

**Prompt usado:**

```markdown
Crie um plano simples para validar a decisão tomada antes de investir muito tempo nela.

Inclua:
- Experimentos ou protótipos sugeridos
- Métricas que devem ser medidas
- Critérios de "go / no-go"
- Tempo estimado para validação
```

---

## Quando Usar Este Workflow

- Escolha de stack tecnológico
- Decisão entre monolito vs microsserviços
- Escolha de banco de dados ou ferramenta de infraestrutura
- Decisões de arquitetura que impactam o time por meses ou anos

---

**Exemplo criado com base em uso real combinando Perplexity + templates deste repositório.**