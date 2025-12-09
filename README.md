# Software de Agendamento de Consultas Online
O Marcador de Consultas é uma aplicação desenvolvida para facilitar o gerenciamento de horários e compromissos em clínicas, consultórios ou serviços que trabalham com agendamento. O objetivo é oferecer uma interface simples, rápida e intuitiva, permitindo que usuários registrem, visualizem, editem e acompanhem consultas sem complexidade.

Com este sistema, é possível organizar informações essenciais dos atendimentos — como data, horário, paciente, status e observações — garantindo maior eficiência e reduzindo falhas no processo de marcação. A solução pode ser utilizada tanto por profissionais quanto por equipes administrativas que precisam coordenar múltiplos agendamentos.

## Funcionalidades Principais

- Cadastro de consultas com informações completas
- Listagem organizada por data
- Edição e exclusão de consultas
- Marcação de status (pendente, confirmada, concluída, cancelada)
- Busca e filtros por paciente, data ou status
- Interface objetiva e pensada para produtividade

## Histórias de Usuário:

1. Agendamento de Consultas
Como paciente,
eu quero marcar uma consulta escolhendo o profissional, o serviço e um horário disponível,
para agendar meu atendimento de forma rápida e sem precisar ligar para a clínica.

2. Visualização de Disponibilidade
Como paciente,
eu quero visualizar facilmente as datas e horários disponíveis,
para escolher o momento mais adequado para minha consulta.

3. Cancelamento/Reagendamento
Como paciente,
eu quero cancelar ou reagendar minha consulta online,
para ter flexibilidade caso meus planos mudem sem precisar entrar em contato por telefone.

4. Recebimento de Lembretes
Como paciente,
eu quero receber lembretes automáticos sobre minha consulta,
para não esquecer o horário e evitar faltas.

5. Cadastro/Login do Paciente
Como paciente,
eu quero me cadastrar e acessar meu perfil,
para gerenciar meus dados pessoais e acompanhar meu histórico de consultas.

6. Gerenciamento de Agenda (Profissional)
Como profissional de saúde,
eu quero configurar meus horários de atendimento no sistema,
para controlar minha disponibilidade para receber pacientes.

7. Visualização da Minha Agenda (Profissional)
Como profissional de saúde,
eu quero visualizar minha agenda completa,
para me organizar e planejar meus atendimentos.

8. Notificações Administrativas
Como administrador da clínica,
eu quero receber alertas sobre mudanças nas agendas ou alta demanda,
para tomar decisões rápidas e manter o fluxo de atendimento organizado.

9. Relatórios e Estatísticas
Como administrador,
eu quero acessar relatórios sobre consultas realizadas, canceladas e taxas de ocupação.

10. Gestão de Usuários
Como administrador,
eu quero cadastrar, editar e desativar contas de profissionais ou pacientes,
para manter o sistema atualizado e seguro.

## Casos de Teste:

1. Agendar Consulta
CT-01 – Agendar consulta com sucesso
Objetivo: verificar se o paciente consegue agendar uma consulta.
Pré-condição: paciente cadastrado e logado; profissionais e horários cadastrados.
Passos:
Acessar a tela de agendamento.
Selecionar um profissional.
Selecionar um serviço (opcional).
Escolher uma data disponível.
Escolher um horário disponível.
Confirmar o agendamento.
Resultado esperado:
→ Consulta exibida como confirmada no painel do paciente e do profissional.

CT-02 – Impedir agendamento em horário já ocupado
Objetivo: garantir que dois pacientes não agendem o mesmo horário.
Pré-condição: horário já reservado.
Passos:
Acessar a tela de agendamentos.
Selecionar um profissional e um horário já agendado.
Tentar confirmar o agendamento.
Resultado esperado:
→ Sistema exibe mensagem de “horário indisponível”.
2. Visualização de Disponibilidade

CT-03 – Exibir apenas horários disponíveis
Objetivo: verificar se o sistema mostra somente horários livres.
Pré-condição: profissional com alguns horários ocupados.
Passos:
Selecionar profissional.
Selecionar data.
Resultado esperado:
→ Apenas horários não ocupados são exibidos.
3. Cancelamento e Reagendamento

CT-04 – Cancelar consulta
Objetivo: permitir que o paciente cancele uma consulta.
Pré-condição: consulta existente e futura.
Passos:
Acessar o menu “Minhas consultas”.
Selecionar uma consulta.
Clicar em “Cancelar consulta”.
Confirmar cancelamento.
Resultado esperado:
→ Consulta marcada como cancelada e horário liberado.

CT-05 – Reagendar consulta
Objetivo: verificar se o paciente pode alterar a data/horário.
Pré-condição: consulta existente; novos horários disponíveis.
Passos:
Acessar “Minhas consultas”.
Selecionar uma consulta ativa.
Clicar em “Reagendar”.
Escolher nova data e horário.
Confirmar alteração.
Resultado esperado:
→ Consulta atualizada com o novo horário.
4. Lembretes de Consulta

CT-06 – Enviar lembrete automático
Objetivo: validar o envio automático de lembretes.
Pré-condição: consulta marcada para as próximas 24 horas.
Passos:
Registrar consulta.
Aguardar o tempo configurado para o lembrete.
Resultado esperado:
→ Paciente recebe lembrete (e-mail/SMS/notificação push).
5. Autenticação

CT-07 – Login com credenciais válidas
Objetivo: verificar autenticação correta.
Pré-condição: usuário cadastrado.
Passos:
Inserir e-mail correto.
Inserir senha correta.
Clicar em “Entrar”.
Resultado esperado:
→ Acesso liberado ao painel do usuário.

CT-08 – Bloqueio após tentativas inválidas
Objetivo: testar política de segurança.
Pré-condição: usuário cadastrado.
Passos:
Inserir senha incorreta 5 vezes.
Resultado esperado:
→ Conta temporariamente bloqueada.
6. Painel do Profissional

CT-09 – Visualizar agenda completa
Objetivo: verificar se o profissional consegue ver sua agenda.
Pré-condição: consultas cadastradas.
Passos:
Entrar como profissional.
Acessar “Minha agenda”.
Resultado esperado:
→ Sistema exibe todas as consultas por data e horário.
7. Administração

CT-10 – Gerar relatório de consultas
Objetivo: validar geração de relatórios.
Pré-condição: consultas realizadas e canceladas no sistema.
Passos:
Acessar painel administrativo.
Selecionar “Relatórios”.
Escolher período.
Gerar relatório.
Resultado esperado:
→ Relatório exibindo quantidade de consultas, cancelamentos e ocupação.
para avaliar o desempenho e planejar melhorias na gestão.


