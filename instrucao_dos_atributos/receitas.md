  <div align="center">
      <img src="https://img.icons8.com/?size=100&id=13HpMwhzW71Q&format=png&color=000000" width="200"/>

  # Receitas

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
    <td align="center"><strong>id_receita</strong></td>
    <td align="center">Identificador único da prescrição</td>
    <td align="center">Permite rastreamento e referência única a cada receita no sistema, facilitando busca, auditoria e controle, especialmente importante para medicamentos controlados e fiscalização sanitária.</td>
  </tr>
  <tr>
    <td align="center"><strong>nome_medico</strong></td>
    <td align="center">Nome completo do médico prescritor</td>
    <td align="center">Identifica o profissional responsável pela prescrição, garantindo responsabilidade legal e técnica pelo tratamento indicado. Essencial para contato em caso de dúvidas e para validação da receita.</td>
  </tr>
  <tr>
    <td align="center"><strong>documento.crm</strong></td>
    <td align="center">Registro do médico no Conselho Regional de Medicina</td>
    <td align="center">Comprova habilitação legal do profissional para prescrever medicamentos. Documento obrigatório em todas as prescrições, permitindo verificação da regularidade do médico junto ao órgão regulador.</td>
  </tr>
  <tr>
    <td align="center"><strong>nome_paciente</strong></td>
    <td align="center">Nome completo do paciente</td>
    <td align="center">Identifica inequivocamente o destinatário da prescrição, evitando trocas de medicação entre pacientes e garantindo que o tratamento seja administrado à pessoa correta.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_responsaveis</strong></td>
    <td align="center">Identificador do responsável pela prescrição no sistema</td>
    <td align="center">Vincula a receita ao registro interno do profissional no sistema hospitalar, facilitando análises de produtividade, padrões de prescrição e responsabilização técnica.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_paciente</strong></td>
    <td align="center">Identificador único do paciente no sistema</td>
    <td align="center">Estabelece relação entre a receita e o registro do paciente no sistema, permitindo construção do histórico farmacoterapêutico completo e análise longitudinal dos tratamentos prescritos ao longo do tempo.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_prescrição</strong></td>
    <td align="center">Data em que a receita foi emitida</td>
    <td align="center">Marca o início formal do tratamento e determina a contagem de validade da prescrição. Crucial para avaliação da atualidade do tratamento e contextualização temporal do quadro clínico.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_validade</strong></td>
    <td align="center">Data limite para dispensação da receita</td>
    <td align="center">Define o período durante o qual a receita pode ser utilizada para retirada dos medicamentos. Especialmente importante para medicamentos controlados, evitando uso prolongado sem reavaliação médica.</td>
  </tr>
  <tr>
    <td align="center"><strong>medicamentos.id</strong></td>
    <td align="center">Código identificador do medicamento</td>
    <td align="center">Vincula a prescrição ao cadastro de medicamentos do sistema, garantindo precisão na dispensação e possibilitando verificações automáticas de interações medicamentosas e controle de estoque.</td>
  </tr>
  <tr>
    <td align="center"><strong>medicamentos.dosagem</strong></td>
    <td align="center">Quantidade do medicamento a ser administrada</td>
    <td align="center">Especifica a concentração exata do princípio ativo para cada administração, fundamental para eficácia terapêutica e prevenção de subdosagem ou toxicidade por superdosagem.</td>
  </tr>
  <tr>
    <td align="center"><strong>medicamentos.via</strong></td>
    <td align="center">Rota de administração do medicamento</td>
    <td align="center">Define como o medicamento deve ser administrado (oral, intravenosa, retal, etc.), afetando diretamente a velocidade de absorção, biodisponibilidade e potenciais efeitos adversos do tratamento.</td>
  </tr>
  <tr>
    <td align="center"><strong>medicamentos.frequencia</strong></td>
    <td align="center">Intervalos e modo de administração</td>
    <td align="center">Estabelece o ritmo de administração para manter níveis terapêuticos adequados no organismo. Crítico para medicamentos com meia-vida curta ou que exigem concentrações plasmáticas estáveis.</td>
  </tr>
  <tr>
    <td align="center"><strong>medicamentos.duracao</strong></td>
    <td align="center">Período total do tratamento</td>
    <td align="center">Determina por quanto tempo o medicamento deve ser utilizado, essencial para completar o ciclo terapêutico, evitar resistência microbiana (no caso de antibióticos) e prevenir dependência em medicamentos controlados.</td>
  </tr>
  <tr>
    <td align="center"><strong>observacao</strong></td>
    <td align="center">Instruções adicionais sobre o tratamento</td>
    <td align="center">Fornece orientações específicas como restrições alimentares, precauções especiais ou condições de uso que aumentam a segurança e eficácia do tratamento, complementando as informações básicas da prescrição.</td>
  </tr>
  <tr>
    <td align="center"><strong>dispensação.data</strong></td>
    <td align="center">Data em que o medicamento foi retirado</td>
    <td align="center">Registra quando o paciente efetivamente obteve o medicamento, permitindo monitorar adesão ao tratamento e calcular o período esperado de uso antes da necessidade de renovação.</td>
  </tr>
  <tr>
    <td align="center"><strong>dispensação.farmacia</strong></td>
    <td align="center">Estabelecimento onde o medicamento foi dispensado</td>
    <td align="center">Identifica o local responsável pela entrega, importante para rastreabilidade em caso de problemas com o medicamento, recalls de lotes ou necessidade de orientações complementares ao paciente.</td>
  </tr>
  <tr>
    <td align="center"><strong>dispensação.responsavel_dispensacao</strong></td>
    <td align="center">Profissional que realizou a entrega do medicamento</td>
    <td align="center">Documenta o farmacêutico responsável pela dispensação, estabelecendo responsabilidade técnica pelo fornecimento correto, orientações de uso e verificação final de possíveis interações ou contraindicações.</td>
  </tr>
</table>
</div>