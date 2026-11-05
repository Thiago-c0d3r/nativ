# NATIV — Visão e Escopo do Produto

**Versão:** 0.2  
**Etapa:** Product Discovery  
**Status:** Levantamento inicial consolidado

## 1. Visão do produto

O Nativ é uma plataforma de gestão, organização e acompanhamento de relacionamentos de discipulado cristão.

Seu objetivo é facilitar a organização entre discipuladores e discípulos, permitindo administrar vínculos, encontros, propósitos, tarefas e históricos de acompanhamento.

A tecnologia serve ao relacionamento humano, sem substituir a conversa, a responsabilidade pessoal ou a centralidade de Cristo no discipulado.

## 2. Público inicial

A primeira versão será direcionada a uma igreja.

Existem dois perfis principais:

- **Discipulador:** acompanha, organiza e administra os relacionamentos de discipulado.
- **Discípulo:** participa do acompanhamento e consulta seus compromissos.

## 3. Relacionamento entre discipulador e discípulo

### 3.1 Cardinalidade

O relacionamento segue uma associação de um para muitos (1:N):

- Um discipulador pode acompanhar vários discípulos.
- Cada discípulo pode possuir apenas um discipulador ativo por vez.

### 3.2 Formação do relacionamento

O vínculo pode começar de duas maneiras:

1. O discipulador procura alguém e pergunta se existe interesse em iniciar o discipulado.
2. A pessoa procura um líder e manifesta interesse em iniciar.

O relacionamento depende da concordância dos envolvidos.

### 3.3 Troca de discipulador

No início do relacionamento, pode acontecer de o discípulo não se adequar ao discipulador.

Nesse caso, existe a possibilidade de troca de discipulador.

A troca deve preservar o histórico dos vínculos anteriores, sem permitir que o discípulo tenha dois discipuladores ativos simultaneamente.

## 4. Encontros

- Os encontros acontecem mensalmente.
- Tanto o discipulador quanto o discípulo podem propor uma data.
- O encontro precisa respeitar a disponibilidade de ambos.
- O sistema deverá permitir organizar os encontros e consultar seu histórico.

## 5. Acompanhamento: arcos mensais

O acompanhamento será organizado em arcos, representando os períodos mensais.

- O discipulador poderá consultar o histórico completo.
- O discípulo visualizará os itens que ainda precisa realizar.
- Quando todas as missões do período forem concluídas, o arco deixa de aparecer como pendência atual.
- Itens ainda pendentes continuam para o próximo arco.

## 6. Propósitos

Propósitos são compromissos de acompanhamento definidos pelo discipulador, após conversa e alinhamento com o discípulo durante o encontro.

Exemplos:
- Desenvolver uma rotina de oração.
- Estabelecer um período de jejum.
- Trabalhar um propósito específico durante determinado período.

### Regras de negócio

- Somente o discipulador cadastra propósitos.
- Ambos podem consultar.
- O discípulo registra sua confirmação de conclusão.
- O discipulador também registra sua confirmação.
- O propósito só é concluído quando os dois confirmam.
- Propósitos pendentes continuam nos próximos arcos.
- Propósitos concluídos permanecem no histórico.
- A conclusão exige unanimidade entre os envolvidos.

## 7. Tarefas

Tarefas são atividades práticas estabelecidas pelo discipulador em alinhamento com o discípulo.

Exemplos:
- Ler determinado livro.
- Ler capítulos específicos.
- Realizar uma atividade combinada durante o encontro.

### Regras de negócio

- Somente o discipulador cadastra tarefas.
- Ambos podem consultar.
- Somente o discípulo pode marcar uma tarefa como concluída.
- O discípulo pode desfazer uma conclusão registrada por engano.
- Tarefas pendentes continuam nos próximos arcos.
- A conclusão não exige confirmação do discipulador.

## 8. Histórico e permissões

O sistema deverá preservar registros de conclusão, incluindo:

- Data e horário da confirmação.
- Responsável pela confirmação.
- Tipo de registro (propósito ou tarefa).
- Histórico de alterações relevantes.

O discipulador terá acesso ao histórico completo do acompanhamento.

O discípulo terá acesso aos itens que ainda precisa realizar, conforme as regras de visualização definidas.

## 9. Gerenciamento de registros

O discipulador poderá realizar operações de cadastro, consulta, atualização e exclusão de propósitos e tarefas.

Regras:

- O discipulador pode excluir ou cancelar itens enquanto estiverem pendentes.
- Itens concluídos não poderão ser excluídos pelo CRUD convencional.
- Registros históricos devem ser preservados.
- A exclusão deverá considerar exclusão lógica (soft delete), em vez de remoção definitiva do banco de dados.

## 10. Comunicação

A comunicação entre os participantes será externa à plataforma, inicialmente utilizando o WhatsApp como canal de contato.

O Nativ não terá chat próprio no escopo inicial.

## 11. Escopo inicial do MVP

- Gestão de usuários e perfis.
- Gestão de relacionamentos de discipulado.
- Solicitações e convites.
- Possibilidade de troca de discipulador.
- Controle de um discipulador ativo por discípulo.
- Histórico de vínculos anteriores.
- Organização dos encontros mensais.
- Registro de propósitos.
- Registro de tarefas.
- Arcos mensais.
- Acompanhamento de conclusão.
- Histórico de acompanhamento.
- Acesso externo ao WhatsApp.

## 12. Fora do escopo inicial

- Chat interno.
- Biblioteca própria de estudos bíblicos.
- Cursos ou trilhas teológicas.
- Gamificação espiritual.
- Pontuação de espiritualidade.
- Inteligência artificial para avaliar o discipulado.

## 13. Pontos que ainda precisam de validação

- Como será implementada a disponibilidade dos participantes.
- Como será operacionalizada a troca de discipulador.
- Quais informações serão editáveis após o cadastro.
- Como serão tratadas as permissões e a privacidade das observações dos encontros.
- Como os usuários serão cadastrados e autorizados pela igreja.
- Como será definido o encerramento e a transição dos arcos mensais.

## 14. Princípio do produto

O Nativ organiza o acompanhamento, mas não substitui o discipulado.

**Pessoas formando pessoas, fundamentadas na Palavra.**