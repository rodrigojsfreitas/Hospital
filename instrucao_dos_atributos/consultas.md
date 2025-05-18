<div align="center">
<img src="https://img.icons8.com/color/48/000000/health-checkup.png" width="200"/>

# Consultas

</div>

---

<div align="center">
<table align="center" align="center">
  <tr>
    <th align="center">Atributo</th>
    <th align="center">Descrição</th>
    <th align="center">Motivo/Importância</th>
  </tr>
  <tr>
    <td align="center"><strong>id_consulta</strong></td>
    <td align="center">Identificador único da consulta</td>
    <td align="center">Permite rastreamento único de cada atendimento realizado no sistema, facilitando referências em relatórios, faturamento e auditoria. O formato alfanumérico (ex: "jfoapjfa1331") garante unicidade mesmo em ambientes com múltiplos sistemas integrados.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_paciente</strong></td>
    <td align="center">Identificador do paciente atendido</td>
    <td align="center">Estabelece a conexão entre o atendimento e o registro do paciente, permitindo construção do histórico médico completo, análise de frequência de visitas e identificação de padrões de utilização do serviço por parte do paciente.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_responsavel</strong></td>
    <td align="center">Array de IDs dos profissionais responsáveis</td>
    <td align="center">Registra quais profissionais (médicos, enfermeiros) participaram da consulta, estabelecendo responsabilidade legal e administrativa. O formato de array permite registrar consultas multidisciplinares ou trocas de responsáveis durante um mesmo atendimento.</td>
  </tr>
  <tr>
    <td align="center"><strong>especialidade</strong></td>
    <td align="center">Código da especialidade médica</td>
    <td align="center">Categoriza o tipo de atendimento realizado, facilitando direcionamento para setores específicos, análise de demanda por especialidade, gestão de recursos especializados e faturamento adequado conforme tabelas de procedimentos.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_entrada</strong></td>
    <td align="center">Data e hora reais de início da consulta</td>
    <td align="center">Registra o momento exato em que o atendimento efetivamente começou, essencial para análise de pontualidade, cálculo de tempo de espera, gestão de ocupação e auditoria de eventos assistenciais. O formato ISO com indicador de fuso horário garante precisão temporal.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_prevista_entrada</strong></td>
    <td align="center">Data e hora agendadas para a consulta</td>
    <td align="center">Documenta quando o atendimento foi originalmente agendado, permitindo comparação com horário real para análises de pontualidade, eficiência operacional e adequação da grade de agendamento às necessidades reais.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_prevista_saida</strong></td>
    <td align="center">Data e hora previstas para término</td>
    <td align="center">Estabelece a duração esperada do atendimento, crucial para planejamento de recursos, otimização de agendas e estimativa de ocupação de consultórios. Permite identificar atendimentos que demandam mais tempo que o previsto para ajustes no planejamento.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_saida</strong></td>
    <td align="center">Data e hora reais de término da consulta</td>
    <td align="center">Registra o momento exato em que o atendimento foi concluído, possibilitando cálculo preciso da duração real das consultas, análise de produtividade dos profissionais e identificação de gargalos no fluxo assistencial.</td>
  </tr>
</table>
</div>