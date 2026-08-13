# Projeto de Interação Humano-Computador (IHC)

## Identificação

**Título do projeto:** XAI-ALZHEIMER INTERFACE  
**TCC/projeto de origem:** M-XAI Net: Um Framework Multimodal de Inteligência Artificial Explicável para Diagnóstico de Doença de Alzheimer  
**Orientador(a):** Murillo Freitas Bouzon  
**Disciplina:** Interação Humano-Computador  
**Instituição:** FEI  
**Semestre:** 8° Semestre

### Equipe

| Nome completo | Matrícula | GitHub | Responsabilidade principal no projeto |
|---|---:|---|---|
| Paulo Hudson | 22.222.013-9 | Unifpsilva |  |
| Ana Carolina | {{matrícula}} | {{@usuario}} |
| Raphael | {{matrícula}} | {{@usuario}} |
| Nathan | {{matrícula}} | {{@usuario}} |

## Resumo do produto

O Problema Central é a opacidade algorítmica (caixa preta) das tecnologias de i.a no diagnóstico precoce da doença de Alzheimer, o que gera desconfiança e impede a adoção dessas ferramentas no contexto clínico e hospitalar de alto risco.
O Usuário final é o médico especialista ou clínico geral. 
O Produto para resolver essa dor é o M-XAI Net, um sistema de suporte que opera como um dashboard usando i.a explicável híbrida (HXAI). A interação funciona assim: O médico insere os dados textuais e a ressonância magnética do paciente no software e, em resposta, interage com uma tela unificada que exibe não apenas o diagnóstico, mas a justificativa exata da máquina através dos mapas de calor (GRAD-CAM) e gráficos de peso (SHAP), permitindo auditar e validar a decisão antes de prescrever o tratamento.

## Como usar este repositório

1. Leia primeiro o [Guia de uso e apresentação](GUIA_DE_USO.md).
2. Preencha as entregas na ordem em que forem trabalhadas na disciplina.
3. Em toda entrega individual, **identifique o autor** da solução.
4. Salve imagens, diagramas e evidências em [`assets/`](assets/README.md), com nomes descritivos.
5. Mantenha a [Matriz de rastreabilidade](RASTREABILIDADE.md) atualizada: uma boa entrega de IHC deve ser coerente com as anteriores e com as posteriores.
6. Antes de cada entrega, revise o checklist específico do arquivo e o [Checklist final do projeto](CHECKLIST_FINAL.md).

## Entregas

| # | Entrega | Quantidade mínima / responsabilidade | Status |
|---:|---|---|---|
| 1 | [Conhecendo o problema](docs/01_conhecendo_o_problema.md) | 1 solução consolidada por equipe | ⬜ |
| 2 | [Público-alvo e análise de concorrência](docs/02_analise_concorrencia.md) | no mínimo 1 concorrente/interface representativa por integrante + síntese da equipe | ⬜ |
| 3 | [Personas, empatia, contexto e jornada](docs/03_personas_contexto_jornada.md) | 1 persona por integrante; demais artefatos consolidados por equipe | ⬜ |
| 4 | [Cenários de análise/problema](docs/04_cenarios_problema.md) | 1 solução completa por integrante | ⬜ |
| 5 | [Análise de tarefas: HTA, GOMS e CTT](docs/05_analise_tarefas.md) | cada integrante: pelo menos 1 HTA + 1 GOMS + 1 CTT | ⬜ |
| 6 | [Prototipação em papel](docs/06_prototipacao_papel.md) | 1 protótipo integrado por equipe | ⬜ |
| 7 | [Coleta de dados e aspectos éticos](docs/07_coleta_dados.md) | soluções individuais + técnicas distintas; questionário deve estar entre as técnicas | ⬜ |
| 8 | [Ciclo de vida e engenharia de usabilidade](docs/08_engenharia_usabilidade.md) | 1 solução consolidada por equipe | ⬜ |
| 9 | [Modelo conceitual e design centrado na comunicação](docs/09_modelo_conceitual.md) | soluções individuais + consolidação dos objetivos/signos | ⬜ |
| 10 | [MoLIC](docs/10_molic.md) | 1 diagrama completo por integrante | ⬜ |
| 11 | [Protótipo no Figma](docs/11_figma.md) | 1 protótipo integrado por equipe, cobrindo os fluxos modelados | ⬜ |
| 12 | [Planejamento da avaliação — DECIDE](docs/12_planejamento_avaliacao.md) | 1 plano consolidado por equipe | ⬜ |
| 13 | [Avaliação heurística](docs/13_avaliacao_heuristica.md) | 1 avaliação completa por integrante, cobrindo todas as telas e as 10 heurísticas | ⬜ |
| 14 | [Avaliação por observação de usuários](docs/14_observacao_usuario.md) | avaliação consolidada; nº de participantes finais = nº de integrantes | ⬜ |

> **Importante:** se o docente definir quantidade diferente para a turma/semestre, a orientação da disciplina prevalece. Registre a alteração no início do arquivo da entrega.

## Visão de continuidade do projeto

O projeto deve formar uma cadeia de evidências:

**Problema → público/contexto → necessidades → personas → cenários → tarefas → modelo conceitual → MoLIC → protótipo → planejamento → inspeção → teste com usuários → melhorias.**

Uma entrega não deve “reiniciar” o projeto. Se uma persona tem um objetivo importante, esse objetivo deve aparecer em cenários/tarefas; se a tarefa foi modelada em MoLIC, deve existir no Figma; se um problema é encontrado na avaliação, deve haver evidência e proposta de correção.

## Documentos de apoio

- [Guia de uso e apresentação](GUIA_DE_USO.md)
- [Matriz de rastreabilidade](RASTREABILIDADE.md)
- [Checklist final](CHECKLIST_FINAL.md)
- [Bibliografia de IHC](BIBLIOGRAFIA.md)
- [Orientações de contribuição no GitHub](CONTRIBUTING.md)
- [Instrumentos reutilizáveis](instrumentos/README.md)
