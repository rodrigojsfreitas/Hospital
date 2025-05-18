 <div align="center">

 <img src="https://img.icons8.com/color/48/000000/doctor-male.png" width="200"/>


 # Medicos

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
    <td align="center"><strong>uuid_medico</strong></td>
    <td align="center">Identificador único universal</td>
    <td align="center">Garante identificação única do médico no sistema e entre diferentes sistemas, prevenindo duplicações mesmo em ambientes distribuídos. Segue o formato padrão UUID.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_medico</strong></td>
    <td align="center">Código alfanumérico simplificado</td>
    <td align="center">Facilita a referência ao médico em comunicações internas, relatórios e atendimentos, sendo mais fácil de memorizar que o UUID. O prefixo "med" seguido pelo estado ("sp") e número sequencial permite identificação rápida.</td>
  </tr>
  <tr>
    <td align="center"><strong>nome</strong></td>
    <td align="center">Nome completo do médico</td>
    <td align="center">Identificação primária usada em todas as interações com pacientes, documentos oficiais e comunicações institucionais.</td>
  </tr>
  <tr>
    <td align="center"><strong>data_nascimento</strong></td>
    <td align="center">Data de nascimento no formato ISO</td>
    <td align="center">Permite cálculo automático da idade, essencial para análise demográfica do corpo médico, verificação de aposentadoria e planejamento de sucessão profissional.</td>
  </tr>
  <tr>
    <td align="center"><strong>tipo</strong></td>
    <td align="center">Classificação do médico (M0, M1, M2)</td>
    <td align="center">Indica o nível hierárquico ou tipo de contratação do médico, o que determina responsabilidades, remuneração e escopo de atuação.</td>
  </tr>
  <tr>
    <td align="center"><strong>especialidades</strong></td>
    <td align="center">Array de códigos de especialidades médicas</td>
    <td align="center">Define as áreas de atuação do médico, permitindo direcionar pacientes de acordo com suas necessidades específicas, organizar escalas de plantão e distribuir casos adequadamente.</td>
  </tr>
  <tr>
    <td align="center"><strong>contato.telefone</strong></td>
    <td align="center">Número de telefone com DDD</td>
    <td align="center">Permite contato direto em situações de emergência, alterações de escala ou comunicações urgentes sobre pacientes.</td>
  </tr>
  <tr>
    <td align="center"><strong>contato.email</strong></td>
    <td align="center">Endereço de e-mail</td>
    <td align="center">Canal de comunicação formal para envio de relatórios, notificações administrativas, atualizações de protocolos e agendamentos.</td>
  </tr>
  <tr>
    <td align="center"><strong>status</strong></td>
    <td align="center">Situação atual do médico (Ativo/Inativo)</td>
    <td align="center">Indica se o profissional está disponível para atendimentos ou temporariamente/permanentemente afastado, permitindo gestão adequada de recursos humanos.</td>
  </tr>
  <tr>
    <td align="center"><strong>em_atividade</strong></td>
    <td align="center">Status atual de serviço (booleano)</td>
    <td align="center">Flag que indica se o médico está trabalhando no momento (em plantão ou expediente). Permite rastreamento em tempo real para encaminhamentos urgentes e gestão de escala.</td>
  </tr>
  <tr>
    <td align="center"><strong>fila_de_pacientes</strong></td>
    <td align="center">Lista de IDs de pacientes aguardando</td>
    <td align="center">Controla pacientes na fila de espera do médico, essencial para organização do fluxo de atendimento e gestão de tempo. Permite priorização e redistribuição quando necessário.</td>
  </tr>
  <tr>
    <td  align="center"><strong>documentos.cpf</strong></td>
    <td align="center">Cadastro de Pessoa Física</td>
    <td align="center">Identificador fiscal necessário para processos administrativos, folha de pagamento, emissão de notas fiscais e declarações tributárias.</td>
  </tr>
  <tr>
    <td align="center"><strong>documentos.crm</strong></td>
    <td align="center">Registro no Conselho Regional de Medicina</td>
    <td align="center">Documento legal obrigatório que comprova habilitação profissional. O prefixo "SP" indica o estado de registro, essencial para validação da autorização para exercício da medicina.</td>
  </tr>
  <tr>
    <td align="center"><strong>id_consultas</strong></td>
    <td align="center">Lista de identificadores de consultas</td>
    <td align="center">Registra o histórico de atendimentos realizados pelo médico, permitindo análise de produtividade, distribuição de carga de trabalho e acesso rápido ao histórico de casos atendidos.</td>
  </tr>
</table>

# Tipos e Especialidades
  
  <table align="center" style="margin: 0 auto;">
    <tr>
      <td width="50%" valign="top">
        <h3 align="center">Tipos de Médicos</h3>
        <table align="center" border="1" cellspacing="0" cellpadding="8">
          <thead>
            <tr bgcolor="#f0f0f0">
              <th>Tipo</th>
              <th>Descrição</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td align="center"><b>M0</b></td>
              <td align="center">Clínico Geral</td>
            </tr>
            <tr>
              <td align="center"><b>M1</b></td>
              <td align="center">Dermatologista</td>
            </tr>
            <tr>
              <td align="center"><b>M2</b></td>
              <td align="center">Pediatra</td>
            </tr>
            <tr>
              <td align="center"><b>M3</b></td>
              <td align="center">Ginecologista</td>
            </tr>
            <tr>
              <td align="center"><b>M4</b></td>
              <td align="center">Cirurgião</td>
            </tr>
            <tr>
              <td align="center"><b>M5</b></td>
              <td align="center">Oftalmologista</td>
            </tr>
          </tbody>
        </table>
      </td>
      <td width="50%" valign="top">
        <h3 align="center">Especialidades</h3>
        <table align="center" border="1" cellspacing="0" cellpadding="8">
          <thead>
            <tr bgcolor="#f0f0f0">
              <th>Especialidade</th>
              <th>Descrição</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td align="center"><b>A</b></td>
              <td align="center">Dermatologia</td>
            </tr>
            <tr>
              <td align="center"><b>B</b></td>
              <td align="center">Pediatria</td>
            </tr>
            <tr>
              <td align="center"><b>C</b></td>
              <td align="center">Urologia</td>
            </tr>
            <tr>
              <td align="center"><b>D</b></td>
              <td align="center">Oftalmologia</td>
            </tr>
            <tr>
              <td align="center"><b>E</b></td>
              <td align="center">Neurologia</td>
            </tr>
            <tr>
              <td align="center"><b>F</b></td>
              <td align="center">Cardiologia</td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
  </table>