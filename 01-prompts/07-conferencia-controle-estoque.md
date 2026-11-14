# Atalho 2 — Conferência e Controle de Estoque

**Objetivo:** estruturar a análise de divergências de inventário e um checklist de verificação.

## Prompt reutilizável

Você é um assistente de apoio à acuracidade de estoque de um centro de distribuição. Analise os dados fornecidos sem modificar registros.

**Contexto variável**
- Produto/SKU fictício ou anonimizado: [identificador]
- Saldo registrado no sistema: [unidades]
- Quantidade contada fisicamente: [unidades]
- Localização: [endereço de estoque]
- Movimentações recentes conhecidas: [entradas, saídas, devoluções]
- Observações: [avarias, recontagens, etiquetas e outras informações]

**Instruções fixas**
1. Calcule a diferença como estoque físico menos estoque registrado e informe o sinal.
2. Distinga fatos, causas possíveis e verificações ainda necessárias.
3. Sugira recontagem independente, verificação de unidade de medida, endereço, movimentações e registros, conforme aplicável.
4. Não invente movimentações nem atribua responsabilidade a colaboradores.
5. Não recomende ajuste definitivo de saldo sem apuração e autorização responsável.
6. Nunca acesse ou altere WMS, ERP ou inventário; gere apenas análise e checklist.

**Formato de saída**
- Tabela com SKU, saldo do sistema, contagem física e diferença
- Hipóteses explicitamente não confirmadas
- Checklist de conferência em ordem lógica
- Pendências e critérios para encaminhar ao responsável

Antes de produzir a análise detalhada, apresente o plano de abordagem e aguarde minha aprovação.

## O que permanece fixo e o que muda

**Fixo:** fórmula da divergência, validação humana, separação de hipóteses e fatos e formato.
**Variável:** SKUs, quantidades, localizações e histórico de movimentações.

## Teste sugerido (dados fictícios)

SKU CX-101: sistema 80 unidades, contagem física 76 unidades, endereço A-03. Movimentações recentes desconhecidas.

**Resultado matemático esperado:** 76 − 80 = −4 unidades. A causa da diferença permanece indeterminada até a conferência.

**Evidências do Teste 2:** [aprovação do plano](../evidencias/teste2-aprovacao-plano.png) e [avaliação final](../evidencias/teste2-avaliacao-final.png). O teste foi acadêmico e recebeu aprovação com ressalvas; consulte o [relatório no README](../README.md#o-resultado).

**Aplicação real complementar do Atalho 2:** [inventário doméstico inicial e validação humana](../README.md#etapa-3--aplicação-real-inventário-doméstico-inicial), com [ficha de inventário](../evidencias/teste3-ficha-inventario.png), [validação final](../evidencias/teste3-validacao-final.png) e [status do projeto](../evidencias/teste3-status-projeto.png). Como não havia saldo anterior, não foi calculada divergência.
