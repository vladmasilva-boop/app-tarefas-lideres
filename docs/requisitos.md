# Requisitos do app de tarefas dos líderes (versão 0.1)

> Documento inicial, para ser ajustado junto com o Vlad antes de qualquer código.

## 1. Objetivo
Organizar as demandas de cada líder de campo em um só lugar, com responsável, prazo e status, para que todos vejam o que está acontecendo na empresa e quais ações estão sendo tomadas.

## 2. Como vai ser usado
- **Fase 1 (teste):** só o Vlad usa. Cria as tarefas, define as datas, confere e atualiza tudo pelo app.
- **Fase 2 (expansão):** os líderes entram, veem as próprias tarefas e atualizam o status.
- **Fase 3 (padrão da empresa):** o app passa a ser a ferramenta oficial de gestão de tarefas e projetos, sem depender de outros aplicativos.

## 3. Quem usa
| Perfil | O que faz |
|---|---|
| Gestor (Vlad) | Cria, edita e apaga tarefas de qualquer líder. Vê tudo. |
| Líder de campo | Vê as suas tarefas, muda o status, escreve comentários. Vê o quadro geral. |

## 4. A tarefa
Campos de cada tarefa:
- Título
- Líder responsável
- **Prazo** (campo mais importante)
- Status: **A fazer**, **Em andamento**, **Feita**, **Em atraso**
- Descrição e comentários (opcional)
- Data de criação e de conclusão (automáticas)

Regra: uma tarefa não concluída cujo prazo já passou vira **Em atraso** automaticamente.

## 5. Telas da versão inicial
1. **Quadro geral:** todas as tarefas, com filtro por líder, status e prazo.
2. **Minhas tarefas / por líder:** a lista de um líder específico, ordenada por prazo.
3. **Nova tarefa / editar tarefa.**
4. **Resumo do dia:** texto pronto por líder (tarefas de hoje, atrasadas e próximas), para copiar e enviar pelo WhatsApp.

## 6. Fora da versão inicial (fases seguintes)
- Envio automático do resumo diário pelo WhatsApp.
- Projetos com subtarefas e datas.
- Login individual para cada líder, com permissões.
- Histórico de alterações (quem mudou o quê e quando).
- Notificações no celular.

## 7. Decisões em aberto
1. Quantos líderes de campo existem hoje e quais são os nomes?
2. O WhatsApp automático será por qual meio (aplicativo oficial de empresas ou envio manual assistido)?
3. Os líderes poderão criar tarefas para si mesmos ou só o Vlad cria?
4. Uma tarefa pode ter mais de um responsável?
5. O app vai rodar só no navegador do celular ou também como aplicativo instalado?
