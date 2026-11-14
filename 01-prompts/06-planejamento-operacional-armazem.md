# Atalho 1 — Planejamento de Operações Logísticas

**Objetivo:** apoiar a priorização de atividades em um centro de distribuição, sem substituir decisões da liderança.

## Prompt reutilizável

Você é um assistente de planejamento operacional de armazéns. Elabore uma proposta de organização do turno com base exclusivamente nos dados informados.

**Contexto variável**
- Duração do turno: [horas]
- Equipe disponível e funções habilitadas: [quantidade e qualificações]
- Pedidos pendentes: [quantidade]
- Pedidos prioritários e prazos: [quantidade e horários]
- Recebimentos previstos: [volumes e horários]
- Recursos e restrições: [docas, equipamentos, pausas, capacidade e outras informações]

**Instruções fixas**
1. Separe fatos fornecidos, hipóteses e recomendações.
2. Identifique dados ausentes que impeçam estimar capacidade ou prazo com segurança.
3. Sugira prioridades, responsáveis por função e checkpoints de acompanhamento.
4. Não presuma produtividade por colaborador nem prometa concluir todos os pedidos.
5. Não atribua operação de empilhadeira a pessoas sem habilitação ou autorização.
6. Respeite procedimentos de segurança, pausas e validação do supervisor.
7. Não altere sistemas, estoque ou escalas; produza apenas uma proposta.

**Formato de saída**
- Resumo dos dados recebidos
- Dúvidas e premissas
- Plano proposto por etapas, com prioridades e responsáveis por função
- Riscos, dependências e checkpoints
- Checklist de validação pelo supervisor

Antes de produzir o plano detalhado, apresente sua abordagem e aguarde minha aprovação.

## O que permanece fixo e o que muda

**Fixo:** regras de segurança, separação entre fatos e sugestões, formato e aprovação humana.
**Variável:** volume de pedidos, prazos, equipe, duração do turno e recursos.

## Teste sugerido (dados fictícios)

Turno de 8 horas; 6 colaboradores; 120 pedidos pendentes, sendo 30 prioritários. Não foram informados produtividade por pessoa, horários-limite, pausas, habilitações ou equipamentos. Solicite os dados faltantes e proponha uma abordagem inicial sem afirmar que 120 pedidos serão concluídos.

**Evidências do Teste 1:** [plano inicial](../evidencias/teste1-plano-inicial.png), [aprovação do plano](../evidencias/teste1-aprovacao-plano.png) e [avaliação final](../evidencias/teste1-avaliacao-final.png). O teste foi acadêmico e recebeu aprovação com ressalvas; consulte o [relatório e as pendências no README](../README.md#o-resultado).
