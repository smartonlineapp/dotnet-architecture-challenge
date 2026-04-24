# Desafio para Tech Lead - Smart Online

## Contexto

Você está trabalhando em um sistema que recebe webhooks de pagamento de um provedor externo.

Cada webhook representa um evento de pagamento e contém um `Id` (único por pagamento) e um valor.

Esse tipo de integração possui dois problemas comuns:

- O provedor pode enviar o mesmo webhook mais de uma vez;
- O processamento pode falhar temporariamente.

Você recebeu o código (Program.cs) durante um code review de um dev do seu time.

## O que fazer

Analise o código e responda:

- O que está errado no código atual?
- Quais problemas isso pode gerar em produção?
- Como você orientaria o dev a resolver?
  - Separe em:
    - **curto prazo** (o que corrigir agora)
    - **médio prazo** (como evoluir a solução)
- Quais trade-offs você considerou nas suas recomendações?
- **Considere obrigatoriamente** os seguintes cenários na análise:
  - Múltiplas instâncias do serviço rodando em paralelo;
  - Indisponibilidade temporária do provedor externo;
  - Volume alto de eventos.

## Regras

- Não precisa escrever código;
- Foque em análise, direcionamento técnico e tomada de decisão;
- Pode sugerir mudanças de arquitetura, se achar necessário;
- Considere apenas o contexto apresentado (sem persistência, a menos que justifique como evolução);
- Evite respostas genéricas. Dê exemplos concretos sempre que possível.

## Diferencial (opcional)

- Como você mediria em produção que a solução está funcionando? (métricas, alarmes, SLOs, o que observar).

## Entrega

- Resposta em texto, formato livre, mas com seções claras (ex: problemas identificados / curto prazo / médio prazo / trade-offs / cenários obrigatórios).
- Pode ser rascunho, vamos discutir junto na entrevista.

## O que avaliamos

- Clareza na identificação dos problemas;
- Capacidade de prever impacto em produção;
- Qualidade do direcionamento técnico;
- Capacidade de priorização (curto vs médio prazo);
- Consistência nos trade-offs apresentados.

## Tempo estimado

20 a 40 minutos
