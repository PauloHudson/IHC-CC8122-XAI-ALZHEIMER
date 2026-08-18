# Entrega 1 — Conhecendo o problema

**Data:** 13/08/2026  
**Status:** 🟨 Em andamento
**Responsabilidade:** Desenvolver uma interface para intermediar o uso do modelo de inteligência artificial explicável que visa auxiliar no diagnóstico da doença de alzheimer por profissionais da área da saúde.

## Objetivo da atividade

Delimitar o produto, os usuários, os benefícios, as funcionalidades e o **contexto de uso** antes de iniciar decisões de interface. Esta entrega funciona como contrato de escopo para as demais.

## 1.1 Membros da equipe

| Nome completo | Matrícula | GitHub |
|---|---:|---|
| Paulo Hudson | 22.222.013-9 | @Paulo Hudson
| Ana Carolina | 22.123.001-4 | @lazzuriana08
| Raphael | 22.123.014-7 | @rapha661
| Nathan | 22.123.028-7 | @NathanGbl

## 1.2 Título original do TCC/projeto

M-XAI: Um framework multimodal de inteligência artificial explicável para diagnóstico da doença de alzheimer

## 1.3 Orientador(a)

Murillo Freitas Bouzon

## 1.4 Está previsto desenvolver interface?

- [X] Sim
- [ ] Não

**Justificativa:**

O projeto tem como intuíto desenvolver uma aplicação web para intermediar a utilização do modelo de inteligência artificial. Por meio da aplicação, o profissional de saúde poderá fornecer dados do paciente, como imagens de exames e informações clínicas, e consultar o resultado produzido pelo modelo juntamente com sua respectiva explicação.

A interface será responsável por apresentar as etapas de envio dos dados, processamento e consulta do resultado de forma adequada ao contexto de utilização por profissionais da área da saúde.

## 1.5 Objetivo do trabalho

Descreva o **resultado que o projeto pretende alcançar**, não apenas a tecnologia a utilizar.

O projeto tem como objetivo desenvolver uma aplicação web que permita a profissionais da área da saúde utilizar um modelo multimodal de inteligência artificial explicável para auxiliar na análise de casos relacionados à doença de Alzheimer.

O sistema deverá permitir que o médico:

forneça dados clínicos do paciente;
envie imagens médicas, como imagens de ressonância magnética ou tomografia, quando aplicável ao modelo;
acompanhe o processamento da solicitação;
consulte a classificação produzida pelo modelo;
visualize os principais fatores considerados pelo modelo para produzir a classificação.

A interface será desenvolvida considerando que o usuário possui conhecimento médico, mas não necessariamente conhecimento em inteligência artificial ou programação. Dessa forma, os elementos necessários para executar cada tarefa deverão ser apresentados utilizando termos compreensíveis dentro do contexto médico e seguindo uma sequência compatível com o fluxo de análise do caso.

O resultado apresentado pelo sistema terá caráter de apoio à decisão, não substituindo a avaliação e a decisão final do profissional de saúde.

## 1.6 Produto final

O que será efetivamente entregue? Ex.: aplicação Web, aplicativo móvel, dashboard, dispositivo interativo, serviço com interface, ferramenta de apoio etc.

Uma aplicação web.

## 1.7 Usuário final

Quem interage diretamente com o produto? Diferencie usuário final, cliente, administrador, especialista e demais stakeholders quando necessário.

<p>Usuário final: Médico</p>
<p>Cliente: Hospital</p>
<p>Administrador: Equipe de TI do hospital</p>
<p>Especialista: Pesquisadores da área médica</p>
<p>Demais stakeholders: Redes de hospitais e convênios</p>

## 1.8 Benefícios para o usuário

| Benefício esperado | Problema/necessidade associada | Para qual usuário |
|---|---|---|
| Facilitar o uso do modelo por trás da interface | A impossibilidade de profissionais da área da saúde de utilizar tecnologias que não são de seu campo de conhecimento | Médico |

## 1.9 Funcionalidades — visão do usuário

Escreva funcionalidades como capacidades observáveis pelo usuário, não como detalhes de backend.

| ID | Funcionalidade | Objetivo do usuário atendido | Prioridade inicial |
|---|---|---|---|
| F01 | Cadastro/login | Poder acessar o sistema | alta |
| F02 | Upload de arquivos | Poder enviar dados do paciente (imagens/planilhas) | alta |
| F03 | Visualização de diagnóstico | Obter resultado do diagnóstico com sua justificativa | alta |

## 1.10 Tecnologias e ferramentas previstas

| Camada/uso | Tecnologia/ferramenta | Por que foi escolhida | Impacto potencial na interação |
|---|---|---|---|
| Interface | **React** | Reutilização e manutenção da interface web. | Responsividade e atualização dos elementos durante as tarefas. |
| Backend | **Node.js** | Desenvolvimento do servidor e criação de APIs utilizando JavaScript. | Processamento das solicitações e comunicação entre as camadas. |
| Banco de dados | **Neon (PostgreSQL)** | Banco PostgreSQL gerenciado em nuvem e integrado à aplicação. | O tempo de acesso aos dados depende da conexão e da disponibilidade do serviço. |

### Interface — React

O **React** será utilizado para o desenvolvimento da interface da aplicação web. A tecnologia permite estruturar a aplicação por meio de componentes reutilizáveis, facilitando a organização, manutenção e evolução das telas.

Na interação com o usuário, o React será responsável pela apresentação dos elementos utilizados nas principais tarefas, como:

- Autenticação;
- Inserção de dados;
- Seleção e envio de arquivos;
- Acompanhamento das solicitações;
- Visualização da classificação;
- Visualização da explicação do modelo.

A utilização do React permitirá atualizar determinados elementos da interface conforme o usuário realiza essas ações, sem a necessidade de recarregar toda a página.

### Backend — Node.js

O **Node.js** será utilizado no desenvolvimento do backend da aplicação. Ele será responsável por processar as requisições realizadas pela interface e estabelecer a comunicação entre o frontend, o banco de dados e os demais componentes necessários ao funcionamento do sistema.

Entre suas responsabilidades estarão:

- Receber as solicitações realizadas pela interface;
- Disponibilizar APIs para comunicação entre as camadas;
- Processar os dados enviados pelo usuário;
- Realizar operações relacionadas ao banco de dados;
- Encaminhar e receber informações necessárias para a análise.

Para o usuário, o desempenho do backend poderá influenciar diretamente o tempo necessário para concluir tarefas como envio de arquivos e consulta dos resultados. Esse tempo poderá variar conforme a conexão de rede e o processamento da solicitação.

### Banco de dados — Neon (PostgreSQL)

O **Neon**, utilizando **PostgreSQL**, será utilizado para o armazenamento estruturado dos dados necessários ao funcionamento da aplicação.

A escolha considera:

- Utilização do PostgreSQL como sistema de gerenciamento de banco de dados;
- Gerenciamento do banco em ambiente de nuvem;
- Possibilidade de integração com o backend;
- Armazenamento estruturado das informações utilizadas pela aplicação.

A interação do usuário poderá ser afetada pelo tempo necessário para consultar ou armazenar informações. Como o banco estará hospedado em nuvem, operações que dependem dele estarão sujeitas à qualidade da conexão de rede e à disponibilidade do serviço.

## 1.11 Contexto de uso

Descreva o contexto de forma estruturada.

### Usuários

Características relevantes para a interação: experiência, conhecimento de domínio, limitações, diversidade, frequência de uso.

### Tarefas e objetivos

Quais tarefas importantes ocorrerão e com que frequência/criticidade?

### Equipamentos e plataforma

Dispositivos, tamanho de tela, entrada/saída, conectividade, restrições de hardware/software.

### Ambiente físico

Iluminação, ruído, mobilidade, privacidade, possibilidade de uso com uma mão, tempo disponível etc.

### Ambiente social e organizacional

Uso individual/coletivo, presença de terceiros, políticas, papéis, responsabilidades, consequências de erro.

## Delimitação inicial

**Dentro do escopo:** {{...}}  
**Fora do escopo:** {{...}}

## Síntese da entrega

O projeto terá como foco uma aplicação web destinada principalmente a médicos, utilizada para intermediar o acesso a um modelo de inteligência artificial explicável voltado ao apoio na análise da doença de Alzheimer. O usuário poderá inserir dados clínicos e imagens médicas, consultar a classificação produzida pelo modelo e visualizar uma justificativa para o resultado. A interface deverá considerar que os usuários possuem conhecimento médico, mas não necessariamente conhecimento técnico em inteligência artificial. O sistema será utilizado principalmente em computadores e em ambientes profissionais, como hospitais e clínicas. Devido à criticidade do contexto de saúde, a apresentação dos resultados deverá ser clara e objetiva, deixando evidente que o sistema atua como ferramenta de apoio à decisão e não substitui a avaliação médica. Essas definições orientarão as decisões de arquitetura da informação, navegação, acessibilidade e design da interface nas próximas etapas.

## Checklist

- [ ] O problema está descrito sem confundir problema com solução.
- [x] Usuário final está identificado de forma específica.
- [ ] Funcionalidades estão na visão do usuário.
- [ ] Benefícios estão ligados a necessidades reais/hipóteses explícitas.
- [ ] Contexto inclui usuários, tarefas, plataforma e ambientes físico/social.
- [ ] Escopo e limites estão claros.
- [ ] A matriz de rastreabilidade foi iniciada.
