# Meu Kit de IA

Desafio de Projeto da [DIO](https://dio.me): monte o seu kit de IA para o dia a dia e delegue uma tarefa real, com você no comando.

O kit foi criado pelo Expert Bruno Lima com os prompts, templates, checklists e skills usados nas Aulas. Ele não é uma apostila: abra a pasta que resolve o seu problema, copie o modelo, adapte e use.

**Copie → adapte → teste → confira → melhore**

## Como Fazer o Desafio

Você não precisa instalar nada nem saber programar. Tudo acontece no navegador.

1. Clique em **Use this template**, depois em **Create a new repository**. Dê um nome simples, como `meu-kit-de-ia`, deixe **Public** e confirme.
2. Siga os passos abaixo com uma tarefa real da sua semana.
3. Preencha a seção [Minha Entrega](#minha-entrega) da sua cópia e entregue o link dela na DIO.

## Os Passos

1. **Escolha uma tarefa real.** Comece pelo trabalho que se repete na sua semana, como preparar uma reunião ou montar um relatório, e não pela ferramenta.
2. **Pegue um modelo.** Abra a pasta do kit que combina com a sua tarefa. Cada modelo tem um botão de copiar no canto.
3. **Adapte.** Troque o que está entre colchetes pelo seu contexto, objetivo, dados, limites e formato.
4. **Teste.** A primeira resposta é um ponto de partida. Ajuste até funcionar para a sua realidade.
5. **Delegue.** Com o [template de delegação](02-templates/03-delegacao.md), entregue a tarefa à IA. Peça o plano antes de ela começar, acompanhe e valide o resultado.
6. **Confira.** Provável não é o mesmo que verdadeiro. Revise com o [Pare, Confira, Use](03-checklists/01-pare-confira-use.md) antes de usar.

## O Que Tem no Kit

| Pasta | Para que serve |
|---|---|
| [01-prompts](01-prompts) | Pedidos prontos para adaptar: escrita, comunicação, pesquisa, comparação e preparação de reuniões |
| [02-templates](02-templates) | Estruturas para preencher: bom pedido, pesquisa e decisão, e delegação |
| [03-checklists](03-checklists) | Revisão de respostas, de textos e de tarefas delegadas |
| [04-skills](04-skills) | Como criar uma skill, e a Skill Preparador de Reuniões usada nas Aulas |
| [05-delegacao-e-automacao](05-delegacao-e-automacao) | Gatilhos de automação, supervisão e checkpoints |

## Os Frameworks das Aulas

- **Bom pedido:** contexto + instrução + objetivo + formato. Quanto menos a IA precisa adivinhar, melhor você consegue avaliar a resposta.
- **Pesquisa e decisão:** pergunta → pesquisa → critérios → comparação → você. Peça fontes quando precisar de informação externa. A decisão final é sua.
- **Segurança:** pare → confira → use. Valide fatos, números, datas, fontes e contexto.
- **Atalhos reutilizáveis:** criar → testar → ajustar → salvar. Separe as instruções fixas das informações que mudam a cada uso.
- **Delegação:** objetivo + contexto + recursos + limites + sucesso. Autonomia funciona melhor quando o resultado esperado está claro.
- **Supervisão:** definir → delegar → acompanhar → validar. Em tarefas maiores, confira o plano, acompanhe os checkpoints e valide o resultado.

> A IA pode ajudar você a escrever, pesquisar, organizar e executar. A responsabilidade pelo resultado continua sendo sua.

---

## Minha Entrega

Este projeto aplica inteligência artificial ao planejamento de operações de armazém e à conferência de estoque. Os cenários são **fictícios e acadêmicos**. Os testes consistem em interações reais com a IA; não houve execução física, alteração de estoque nem integração com sistemas de gestão.

### Tarefa escolhida e natureza da aplicação

Escolhi o planejamento de um turno de um centro de distribuição como **exercício acadêmico de delegação**, com priorização de pedidos, distribuição de funções, identificação de riscos e checkpoints. O segundo exercício aborda a análise documental de divergência de estoque. **Ambos utilizam dados fictícios**; não constituem execução de uma tarefa real da semana. O enunciado original da DIO solicita uma tarefa real, requisito que ainda precisa ser complementado com uma aplicação autêntica ou esclarecido com a organização do desafio. Não foi registrada aplicação real neste repositório.

### Meus Atalhos

Adaptei e publiquei dois prompts reutilizáveis na pasta `01-prompts`:

**Atalho 1 — Planejamento de Operações Logísticas:** [abrir prompt completo](01-prompts/06-planejamento-operacional-armazem.md). Mantém fixas as regras de segurança, a separação entre fatos e hipóteses e a exigência de aprovação humana. Variam o volume de pedidos, a equipe, os prazos, os equipamentos e a duração do turno. **Situação:** testado; aprovado com ressalvas.

```text
Atue como assistente de planejamento de armazém.
Com base nos pedidos, prioridades, equipe, jornada e recursos informados,
apresente primeiro sua abordagem e aguarde aprovação.
Depois, proponha prioridades, distribuição por função, checkpoints e riscos.
Separe fatos, premissas e recomendações. Não invente produtividade,
não garanta prazos sem dados e não autorize operações inseguras.
```

**Atalho 2 — Conferência e Controle de Estoque:** [abrir prompt completo](01-prompts/07-conferencia-controle-estoque.md). Mantém fixos o cálculo da divergência, a investigação de hipóteses e a proibição de ajustes automáticos. Variam SKU, saldos, localização e movimentações. **Situação:** testado; aprovado com ressalvas. O prompt completo agora exige aprovação do plano antes da análise detalhada.

```text
Atue como assistente de conferência de estoque.
Para cada SKU, compare a contagem física com o saldo do sistema.
Calcule a diferença (físico - sistema), identifique hipóteses não confirmadas
e proponha um checklist de recontagem e investigação.
Não invente movimentações, não atribua culpa e não ajuste o estoque.
Antes da análise detalhada, apresente o plano e aguarde aprovação.
```

### Minha Delegação

A solicitação abaixo foi efetivamente encaminhada à IA no Teste 1:

```text
OBJETIVO
Elaborar um plano de abordagem e, após aprovação, um planejamento
operacional detalhado para um turno fictício de centro de distribuição.

CONTEXTO
120 pedidos pendentes, 30 prioritários, 6 colaboradores e turno de 8 horas.

RECURSOS
Somente os dados fornecidos na conversa e o atalho de planejamento.

LIMITES
Não presumir produtividade, prazos, habilitações ou disponibilidade
de equipamentos. Não realizar operações físicas nem alterar sistemas.
Diferenciar dados conhecidos, hipóteses e recomendações.

SUCESSO
Entregar um plano coerente com prioridades, responsabilidades propostas,
riscos, checkpoints e critérios de validação humana.

Antes de começar, apresente o plano de abordagem e aguarde minha aprovação.
```

**Delegação do Teste 2 — Conferência e Controle de Estoque:**

```text
OBJETIVO
Analisar documentalmente uma divergência fictícia de estoque e preparar
hipóteses, checklist de verificação, pendências e relatório.

CONTEXTO
SKU CX-101; endereço A-03; saldo do sistema informado: 80 unidades;
contagem física informada: 76 unidades; movimentações desconhecidas.

RECURSOS
Somente os dados fictícios fornecidos e o Atalho 2.

LIMITES
Não inventar movimentações ou causas; não atribuir responsabilidades;
não acessar WMS/ERP; não executar recontagem nem ajustar saldos.

SUCESSO
Calcular corretamente a divergência; separar fatos de hipóteses;
produzir checklist, pendências e relatório sujeito a validação humana.

Antes de produzir a análise detalhada, apresente o plano de abordagem
e aguarde minha aprovação.
```

### O Plano da IA

A IA apresentou uma abordagem com cinco etapas: analisar pedidos e prioridades; verificar capacidade operacional; propor distribuição de funções; estabelecer checkpoints; e preparar relatório. Destacou a ausência de informações sobre produtividade, prazos, equipamentos, pausas e habilitações.

**Checkpoint humano:** o plano inicial foi aprovado explicitamente pelo responsável pelo teste antes da geração do planejamento detalhado.

**Evidência visual do Teste 1 — plano e aprovação:** captura autêntica da conversa — **aguardando arquivo fornecido pelo participante**. Não há imagem inserida.

### O Resultado

**Teste 1 — Planejamento operacional (realizado em conversa, cenário fictício).**

A IA produziu uma proposta com alocação hipotética de seis funções, cronograma em janelas de acompanhamento, checkpoints no início, após 2h, 4h, 6h e ao final do turno, indicadores sugeridos e matriz de riscos. O relatório **não afirmou** que todos os 120 pedidos seriam concluídos.

**Validação humana registrada:** *aprovado com ressalvas — ajustes necessários*. Observação do avaliador: “Nem todos os pedidos da conferência humana foram confirmados.”

| Item de conferência | Resultado |
|---|---|
| 1. Prioritários identificados e prazos verificados | Parcial: 30 prioritários identificados; prazos desconhecidos |
| 2. Disponibilidade de estoque conferida | Pendente: não foram fornecidos dados |
| 3. Funções e habilitações verificadas | Pendente: funções propostas, habilitações não confirmadas |
| 4. Pausas e recursos considerados | Parcial: limitações mencionadas, mas não confirmadas |
| 5. Checkpoints e responsáveis definidos | Parcial: checkpoints definidos; responsáveis não confirmados |
| 6. Pendências e riscos registrados | Atendido |
| 7. Nenhuma meta assumida sem evidência | Atendido |

**Ajustes identificados:** solicitar prazos dos pedidos prioritários, capacidade observada, disponibilidade de estoque, equipamentos, qualificações, pausas e responsáveis pelos checkpoints antes de considerar o plano apto para uso operacional.

**Limite do resultado:** o planejamento é apenas uma proposta documental. Não houve separação de pedidos, conferência física, expedição ou atualização de WMS/ERP.

**Evidência visual do Teste 1 — resultado e validação:** captura autêntica da conversa — **aguardando arquivo fornecido pelo participante**. Não há imagem inserida.

**Teste 2 — Conferência e Controle de Estoque (realizado em conversa, cenário fictício).**

**Dados utilizados:** SKU CX-101, localização A-03, saldo informado no sistema de 80 unidades e contagem física informada de 76 unidades. Histórico de movimentações desconhecido.

**Plano apresentado antes da execução:** validação dos dados, proposta de recontagem independente, investigação de hipóteses, checklist e relatório de divergência. O responsável pelo teste **aprovou explicitamente** essa abordagem antes da análise detalhada.

**Resultado documental:** diferença calculada como 76 − 80 = **−4 unidades**, correspondente a 5% do saldo informado. A IA apresentou hipóteses não confirmadas (erro de contagem, movimentação não registrada, endereço incorreto, unidade de medida, avaria ou identificação) e propôs recontagem independente, consulta aos registros e conferência de endereços. Nenhuma causa foi declarada comprovada; nenhum saldo foi ajustado.

**Validação humana registrada:** **aprovado com ressalvas**. Observação do avaliador: “O cálculo e o relatório estão corretos, mas a recontagem física, a consulta às movimentações e a verificação dos endereços permanecem pendentes por se tratar de uma simulação acadêmica.”

| Critério de validação do Teste 2 | Resultado |
|---|---|
| Cálculo da divergência | Atendido: −4 unidades |
| Identificação dos dados fictícios | Atendido: SKU CX-101, endereço A-03 |
| Separação entre fatos e hipóteses | Atendido |
| Checklist e relatório documental | Atendido |
| Unidade de medida e cadastro confirmados | Pendente |
| Recontagem física independente | Não realizada |
| Histórico de movimentações consultado | Não realizado |
| Inspeção de endereços relacionados | Não realizada |
| Alteração de saldo | Não realizada; depende de investigação e autorização humana |

**Limite do resultado:** trata-se de análise documental de números fornecidos para fins acadêmicos. Não houve acesso a WMS/ERP, conferência física, movimentação de mercadorias nem auditoria operacional.

**Evidências visuais do Teste 2:** capturas autênticas do plano inicial e aprovação, do relatório detalhado e da avaliação com ressalvas — **aguardando arquivos fornecidos pelo participante**. Não há imagens inseridas.

### Como Foi para Você

A IA auxiliou na estruturação dos prompts, dos planos e dos relatórios, sem que tenha sido medido tempo economizado. A conferência mostrou que uma resposta organizada não significa que todos os dados operacionais tenham sido verificados. O principal aprendizado até aqui é manter a aprovação e a validação humana como etapas distintas da geração do conteúdo.

**Situação da entrega:** dois atalhos publicados e dois testes acadêmicos realizados e avaliados com ressalvas. As capturas de tela dos planos, aprovações, resultados e avaliações ainda não foram fornecidas nem inseridas. A aplicação em uma tarefa real, prevista no enunciado da DIO, ainda não foi comprovada. Não houve execução física.
