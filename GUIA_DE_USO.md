# Guia de uso, formatação e apresentação

Este guia existe para evitar que o repositório seja apenas um conjunto de respostas soltas. O GitHub deve funcionar como **documentação técnica e acadêmica navegável**, permitindo compreender o raciocínio de projeto e verificar as evidências.

## 1. Padrão de cada entrega

Cada arquivo em `docs/` segue, sempre que aplicável, esta estrutura:

1. **Identificação da entrega** — data, status, autores e escopo.
2. **Objetivo da atividade** — o que o método de IHC pretende descobrir/modelar/avaliar.
3. **Entradas** — quais entregas anteriores fundamentam esta etapa.
4. **Produção** — artefatos, tabelas, diagramas e análise.
5. **Síntese** — o que a equipe aprendeu e que decisão de design decorre da atividade.
6. **Rastreabilidade** — ligação explícita com artefatos anteriores e próximos.
7. **Checklist de qualidade** — revisão antes de concluir.
8. **Referências** — fontes acadêmicas e fontes externas efetivamente utilizadas.

## 2. Identificação de autoria

Entregas individuais devem conter a linha:

`**Autor(a):** Nome completo — matrícula`

Quando houver consolidação, não apague as contribuições individuais. Mostre **quem produziu cada artefato** e depois apresente a síntese da equipe.

## 3. Imagens, diagramas e prints

- Não use imagem minúscula ou ilegível.
- Coloque **legenda** e explique no texto por que a figura é relevante.
- Prefira arquivos locais do repositório a links temporários de anexos externos.
- Nomeie arquivos de forma estável: `hta_buscar_produto.png`, `molic_realizar_saque.png`, `heuristica_h3_tela_pagamento.png`.
- Para diagramas, mantenha **duas versões quando possível**:
  - versão renderizada (`.png` ou `.svg`) para leitura no GitHub;
  - fonte editável (`.drawio`, `.fig`, etc.) para manutenção.
- Em prints de concorrentes e protótipos, não recorte tanto a ponto de perder o contexto da tela.
- Não inclua dados pessoais reais sem necessidade e autorização.

Exemplo:

```md
![HTA — realizar transferência](assets/05_tarefas/hta_transferencia.svg)

*Figura 1 — HTA da tarefa “realizar transferência”. Fonte: elaboração da equipe.*
```

## 4. Tabelas

Use tabelas para **comparar** e **estruturar**, não para esconder textos muito longos. Quando uma célula virar um parágrafo extenso, considere criar subseções e deixar na tabela apenas a síntese.

Toda tabela comparativa deve ter critérios claros. Evite colunas vagas como “bom/ruim” sem justificativa.

## 5. Escrita acadêmica e objetividade

- Defina termos técnicos na primeira ocorrência.
- Distingua **dado**, **interpretação** e **decisão de projeto**.
- Não apresente suposições sobre usuários como fatos. Indique a origem: entrevista, questionário, literatura, análise de concorrência ou hipótese a validar.
- Evite frases genéricas (“a interface deve ser intuitiva”). Diga **para quem**, **em qual tarefa** e **como será verificado**.
- Use a terminologia do método corretamente. Ex.: MoLIC não é um fluxograma de telas; avaliação heurística não substitui teste com usuários.

## 6. Referências

Ao usar uma fonte externa, informe pelo menos: autor/organização, título, ano (quando disponível), link e data de acesso quando pertinente. Referências acadêmicas centrais estão em [BIBLIOGRAFIA.md](BIBLIOGRAFIA.md).

Não confunda “fonte da imagem” com “referência conceitual”. Uma captura de um concorrente precisa indicar o produto e a data; uma definição de método deve ter referência bibliográfica.

## 7. Links externos

Links para Figma, Forms, vídeos e planilhas devem:

- estar com permissão de visualização adequada;
- ser testados em janela anônima antes da entrega;
- ter uma evidência local mínima no GitHub (print, tabela ou resumo), para que a correção não dependa exclusivamente do link externo.

## 8. Consistência entre entregas

Antes de concluir qualquer etapa, responda:

- O público desta entrega é o mesmo definido anteriormente?
- Os objetivos das personas aparecem nos cenários?
- As tarefas analisadas são relevantes para os cenários?
- O modelo conceitual utiliza os mesmos signos e objetivos?
- O MoLIC representa os mesmos objetivos e caminhos?
- O Figma implementa os fluxos do MoLIC?
- As avaliações cobrem justamente esses fluxos/telas?

Use [RASTREABILIDADE.md](RASTREABILIDADE.md) para registrar essas relações.

## 9. Erros frequentes que este template procura evitar

- quantidade de artefatos menor que o número exigido de integrantes;
- ausência do nome do autor em entregas individuais;
- personas genéricas, estereotipadas ou sem relação com dados/evidências;
- cenários de problema que já descrevem a solução;
- HTA, GOMS e CTT usados como desenhos decorativos sem explicação;
- MoLIC reduzido a sequência de telas, sem conversação, alternativas e rupturas;
- Figma sem correspondência com os modelos anteriores;
- avaliação heurística que aplica apenas algumas heurísticas ou só às telas “principais”;
- problemas heurísticos sem print/localização, justificativa de severidade ou solução;
- teste com usuários sem perfil, consentimento, critérios de sucesso, tempos/erros ou evidência;
- conclusão que apenas diz “foi fácil”, sem consolidar achados e mudanças necessárias;
- dependência de links inacessíveis, sem conteúdo equivalente documentado no repositório.

## 10. Estado da entrega

Use um dos estados no topo do arquivo:

- `⬜ não iniciada`
- `🟨 em andamento`
- `🟩 concluída`
- `🟦 revisada após feedback`

Ao revisar após feedback, adicione uma seção **Histórico de revisões** indicando o que mudou.
