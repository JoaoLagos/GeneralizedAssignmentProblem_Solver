# Problema Generalizado de Atribuição (PGA)

## Introdução
O Problema Generalizado de Atribuição (PGA) é um problema clássico de otimização combinatorial que busca encontrar a melhor forma de atribuir um conjunto de tarefas a um conjunto de agentes, de modo a otimizar um determinado critério, como o custo total ou o tempo de conclusão. 

**Exemplo de aplicação:** Alocação de tarefas em projetos, roteamento de veículos, escalonamento de tarefas em sistemas distribuídos.

## Objetivo do Projeto
Este projeto tem como objetivo implentar duas meta-heurísticas diferentes e resolver o problema generalizado de atribuição.

---

## Ideia escolhida:
Até o presente momento, o problema escolhido foi o de **Escalonamento de Motoristas**.

### Cenário

Imagine uma empresa de transporte com uma frota de ônibus que precisa definir as escalas dos motoristas para atender às diversas linhas e horários. Cada linha possui características específicas, como tempo de duração, hora inicial e hora final. Os motoristas possuem diferentes níveis de experiência, que influenciam no seu custo.

### O problema

Como atribuir cada rota/linha a um motorista de forma a maximizar o lucro total levando em conta a custo de cada motorista _m_ para cada tarefa (linha/rota) _t_ e o lucro de cada tarefa (linha/rota) _t_, garantindo que todos os horários sejam cobertos.

### Elementos do PGA nesse cenário

- Tarefas: Cada rota/linha de ônibus representa uma tarefa a ser realizada.
- Agentes: Cada motorista é um agente responsável por executar as tarefas (rotas).
- Matriz de custos: O "custo" de atribuir uma rota a um motorista pode ser o custo do funcionário, por exemplo.
- Restrições:
  - Jornada de trabalho: Cada motorista tem um limite máximo de horas de trabalho por dia e por semana.
  - Cada motorista só pode pegar uma rota/linha que não esteja em conflito de horários com outra que ele já irá executar
- Função objetivo: Maximizar o lucro total.
