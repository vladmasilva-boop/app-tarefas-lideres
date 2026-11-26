# Projeto: Gestão de Tarefas dos Líderes

**Dono:** Vladimir Martins (Vlad), fundador e CEO da Personal Class / Grupo Pratique
**Status:** em uso (fase de teste), construído no Claude entre 19/10 e 26/11/2026
**Objetivo:** tirar a centralização do CEO. Cada líder sabe o que entregar e o que está atrasado, e o Vlad acompanha tudo em um só lugar, sem precisar perguntar a cada um.

---

## 1. Onde fica cada coisa

| O quê | Onde |
|---|---|
| Aplicativo (quadro de tarefas) | https://claude.ai/artifact/Kz8PmEBg6fsbmEhyy2e6FM ("Tarefas dos Líderes de Campo", título na tela "Projetos / Tarefas") |
| Atalho no celular | Adicionado à tela inicial a partir do link acima |
| Dados (líderes e tarefas) | Banco de dados interno do próprio aplicativo, no Claude. Só aparecem para quem entra com a conta que tem acesso. |
| Conversa onde o app foi construído | Conversa "Gestão de tarefas para líderes" (fora de projeto). Para pedir mudanças no app, use essa conversa ou peça a uma conversa nova com o link do app. |
| Resumo diário para WhatsApp | Tarefa agendada "Mensagens diárias dos líderes", seg a sáb às 6h52, com notificação no celular |
| Cópias de segurança | Arquivos `Quadro_de_Tarefas_codigo_v21.html` (código do app) e `Quadro_de_Tarefas_backup_26-11-2026.csv` (todas as tarefas) |

---

## 2. Líderes cadastrados (26/11/2026)

| Líder | Unidade |
|---|---|
| Samuel | Gestor SC |
| Mike | MG |
| Heloísa Piscna | MG |
| Alessandro Single | MG |
| Gabriel | MG |
| Vladimir | Geral |
| Tiago | Obra |
| Valéria - Office Manager | BH (hub de produtos) |

---

## 3. O que o aplicativo faz

**Aba Tarefas**
- Um bloco por líder, que abre e fecha com um toque no nome. No celular os blocos abrem recolhidos. O cabeçalho mostra "X/Y feitas" e um selo de atrasos.
- Status de cada item: ❌ a fazer · ⏰ em andamento · ✅ feita · 🔴 em atraso. Um item vira 🔴 sozinho quando o prazo vence sem conclusão.
- Os quatro números do topo (feitas, em andamento, em atraso, a fazer) funcionam como filtros.
- O período é escolhido nas caixas **De / Até**, com o botão **Semana atual** para voltar. Tarefas atrasadas de antes do período continuam aparecendo.
- Nova tarefa: líder, título e prazo, com atalhos de prazo rápido (Hoje, Amanhã, Quarta, Sexta, Sábado, Próx. segunda).
- Em cada tarefa:
  - **📅** muda o prazo;
  - **Editar** muda título, prazo, líder e quem entrega;
  - **Excluir** pede confirmação;
  - **+ Etapa** quebra a tarefa em subtarefas;
  - **↔** transfere para outro líder;
  - **▲ ▼** (celular) ou arrastar (computador) mudam a prioridade.
- **Etapas (subtarefas):** ficam aninhadas abaixo da tarefa principal, com o selo "▸ 2/5 etapas". Cada etapa tem prazo, status, o **líder que acompanha e cobra** e o campo **🔧 Quem entrega**, para quem executa (pode ser alguém de fora, como Marlon no elétrico ou Rafael na marcenaria).
- **Transferência:** arraste a tarefa até o bloco de outro líder ou use o ↔. A tarefa vai junto com as etapas do mesmo líder, fica marcada "↪ veio de…" por 7 dias e pode ser desfeita no aviso.
- **Prioridade manual:** a ordem que o Vlad define vale no quadro e na mensagem de WhatsApp. Sem ordem definida, a lista mostra primeiro as atrasadas e depois por prazo.
- **Busca no topo:** procura por título, nome de quem entrega, líder ou projeto, ignorando acentos. Tocar no resultado leva direto à tarefa, com destaque em dourado.
- **Botão "Copiar p/ WhatsApp"** em cada líder, e **"Ver mensagem"** para conferir antes.

**Aba Projetos**
- Toda tarefa que tem etapas vira um projeto. A aba mostra barra de progresso, próxima etapa, quem acompanha e quem entrega.
- Semáforo do projeto:
  - 🔴 alguma etapa atrasada;
  - 🟡 etapa vencendo em até 1 dia, ou reta final com menos de 70% concluído;
  - 🟢 em dia;
  - ✔️ todas as etapas feitas.

**Visual:** paleta dourada da Personal Class, com tema claro e escuro. Cabeçalho "Gestão Vladimir · Líderes / Projetos / Tarefas".

---

## 4. Mensagem de WhatsApp (formato atual)

Sem emojis de status. Os itens feitos entram só na contagem, e os atrasados vêm em destaque no topo de cada bloco.

```
Bom dia, Tiago!
Suas missões de 23/11 a 29/11:

*TAREFAS*
- *ATRASADA* · Pilates Buritis — desde sex 30/10
- Sala Pilates - Rio Branco — sex 27/11 (em andamento)

*IMPLEMENTAÇÃO UNIDADE CÉU AZUL - ENTREGAR NA UNIDADE*
Prazo final: seg 30/11 · 2 de 8 etapas feitas
- Projeto Elétrico — qui 26/11 (em andamento)
   entrega: Marlon

*Resumo:* 13 pendentes · 6 atrasadas
Vai me atualizando. 💪
```

- O bloco **APOIO EM OUTROS PROJETOS** aparece quando o líder acompanha etapas de projetos de outro líder.
- O resumo das 6h52 manda primeiro uma linha geral (pendentes, em andamento, atrasados e quem tem mais atrasos) e depois uma mensagem por líder, pronta para copiar.

---

## 5. Projetos e frentes em andamento (26/11/2026)

- **Implementação Unidade Céu Azul** (Tiago, até 30/11): etapas de elétrica (Marlon), marcenaria (Rafael), marketing (Jaqueline), sistema (Samuel), layout/plotagem (Vladimir), regularização de equipe e studio (RH) e fechamento (Vladimir).
- **Layouts das unidades** (Heloísa, até 12/12): 13 layouts, de Lindeia a Cidade Nova.
- **Fechamento de contrato com os Fisioterapeutas** (Valéria, até 04/12): documentação, assinatura dos contratos, contratação da Jaqueline e regularização das salas junto ao Crefito.
- **Estagiários: organização e controle** (Valéria, até 27/11): controle dos estágios e entrevistas.
- **Frentes do Mike:** RH e DP (procedimentos e responsáveis), TI e indicadores diários, contratação do(a) gestor(a) de Pilates e líder de sócios da Personal Class.
- **Contabilidade e Jurídico** (Tiago acompanha): transferência da contabilidade da Single Ouro Preto.

O estado completo e atualizado está sempre no próprio aplicativo. O CSV é uma foto de 26/11.

---

## 6. Pendências e decisões em aberto

1. **Sobreposição Crefito × "Regularização Studio".** Decidir se as duas tarefas são a mesma: a etapa da Valéria (04/12) ou a do Tiago com o RH (28/12).
2. **"Contratar Jaqueline" × "Contratação Gestor(a) Pilates".** Confirmar se a tarefa do Mike pode ser fechada.
3. **Projetos marcados como feitos com etapas abertas:** "5. RH e DP" e "6. TI" do Mike.
4. **Tarefas paradas desde outubro:**
   - Tiago: Buritis, Fernão Dias 2 e Pilates industrial;
   - Vladimir: Recebimento Geraldinho e pagamento ao Léo.
5. **Antes de compartilhar com os líderes:** ajustar as permissões para que eles só atualizem o status e o Vlad continue criando, editando e excluindo. Hoje quem tem acesso pode excluir.

---

## 7. Próximos passos sugeridos (ideias já discutidas)

- Tarefas recorrentes (toda semana).
- Campo de observação por tarefa e foto de comprovação na conclusão.
- Etapa "Validada" pelo Vlad depois do ✅ do líder.
- Modelos de projeto prontos (ex.: abertura de unidade).
- Visão Kanban e fechamento automático de sexta, com o percentual entregue no prazo por líder.
- Mais à frente, se precisar de login próprio para os líderes, envio automático pelo WhatsApp e endereço próprio: migrar para um aplicativo próprio (código no GitHub, banco Supabase/Firebase), usando o código e o CSV deste pacote como ponto de partida.

---

## 8. Como pedir mudanças

Em qualquer conversa do Claude, cole o link do aplicativo e descreva a mudança. Por exemplo: "No quadro https://claude.ai/artifact/Kz8PmEBg6fsbmEhyy2e6FM, quero adicionar um campo de observação nas tarefas". O Claude consegue ler o app, alterar e republicar no mesmo link, sem perder os dados.
