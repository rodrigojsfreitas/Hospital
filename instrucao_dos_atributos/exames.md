  <div align="center">
      <img src="https://img.icons8.com/color/48/000000/microscope.png" width="200"/>

  # Exames
  </div>

---

<div align="center">
<table align="center" style="text-align: center;">
  <tr>
    <th align="center">Atributo</th>
    <th align="center">Descrição</th>
    <th align="center">Motivo/Importância</th>
  </tr>
  <tr>
    <td align="center"><strong>paciente_id</strong></td>
    <td align="center">Identificador único do paciente</td>
    <td align="center">Estabelece vínculo entre o exame e o paciente, permitindo rastreabilidade completa dos exames por paciente e construção do histórico médico. Essencial para evitar erros de identificação em resultados críticos.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_responsavel</strong></td>
    <td align="center">Array com IDs dos médicos solicitantes</td>
    <td align="center">Identifica o profissional que solicitou o exame, estabelecendo responsabilidade técnica e permitindo encaminhamento correto dos resultados. O formato de array possibilita múltiplos solicitantes em casos de juntas médicas.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_entrada</strong></td>
    <td align="center">Data e hora da coleta do exame</td>
    <td align="center">Registra o momento exato da coleta ou realização do procedimento, crucial para avaliação temporal dos resultados, cálculo de tempo de processamento e validação da cronologia do quadro clínico do paciente.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_prevista_alta</strong></td>
    <td align="center">Data e hora estimadas para liberação dos resultados</td>
    <td align="center">Define expectativa de prazo para entrega dos resultados, permitindo planejamento terapêutico adequado, gerenciamento de expectativas do paciente e organização do fluxo de análises no laboratório.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_efetiva_alta</strong></td>
    <td align="center">Data e hora reais de liberação dos resultados</td>
    <td align="center">Documenta quando os resultados foram efetivamente disponibilizados, possibilitando análise de pontualidade do serviço, auditoria de prazos e avaliação do desempenho operacional do laboratório.</td>
  </tr>
  <tr>
    <td align="center"><strong>procedimentos.Procedimento</strong></td>
    <td align="center">Código do procedimento realizado</td>
    <td align="center">Classifica o tipo de intervenção realizada segundo tabelas padronizadas (PD1, PD2, etc.), essencial para faturamento, integração com sistemas de gestão hospitalar e classificação em protocolos assistenciais.</td>
  </tr>
  <tr>
    <td align="center"><strong>procedimentos.Exame</strong></td>
    <td align="center">Tipo específico de exame</td>
    <td align="center">Identifica o teste laboratorial ou diagnóstico específico (TGO, Hemograma, etc.), determinando métodos de análise, valores de referência e significado clínico dos resultados encontrados.</td>
  </tr>
  <tr>
    <td align="center"><strong>quarto_id</strong></td>
    <td align="center">Identificador do quarto do paciente</td>
    <td align="center">Registra a localização do paciente quando internado, facilitando a coleta de amostras, entrega de resultados emergenciais e rastreabilidade de possíveis contaminações em caso de surtos hospitalares.</td>
  </tr>
  <tr>
  <!-- Consertar -->
    <td align="center"><strong>id_dos_responsaveis</strong></td>
    <td align="center">Lista de IDs dos profissionais</td>
    <td align="center">Documenta quais profissionais realizaram a coleta ou auxiliaram no procedimento, estabelecendo cadeia de custódia da amostra, responsabilização técnica e possibilitando contato em caso de necessidade de repetição ou esclarecimentos sobre a coleta.</td>
  </tr>
</table>
</div>