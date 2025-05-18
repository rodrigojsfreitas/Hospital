 <div align="center">

 <img src="https://img.icons8.com/color/48/000000/doctor-male.png" width="200"/>


 # Medicos

 </div>
 
 ---

 <div align="center">
<table align="center" style="text-align: center;">
  <tr>
    <th style="text-align: center;">Atributo</th>
    <th style="text-align: center;">Descrição</th>
    <th style="text-align: center;">Motivo/Importância</th>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>uuid_medico</strong></td>
    <td style="text-align: center;">Identificador único universal</td>
    <td style="text-align: center;">Garante identificação única do médico no sistema e entre diferentes sistemas, prevenindo duplicações mesmo em ambientes distribuídos. Segue o formato padrão UUID.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_medico</strong></td>
    <td style="text-align: center;">Código alfanumérico simplificado</td>
    <td style="text-align: center;">Facilita a referência ao médico em comunicações internas, relatórios e atendimentos, sendo mais fácil de memorizar que o UUID. O prefixo "med" seguido pelo estado ("sp") e número sequencial permite identificação rápida.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>nome</strong></td>
    <td style="text-align: center;">Nome completo do médico</td>
    <td style="text-align: center;">Identificação primária usada em todas as interações com pacientes, documentos oficiais e comunicações institucionais.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>data_nascimento</strong></td>
    <td style="text-align: center;">Data de nascimento no formato ISO</td>
    <td style="text-align: center;">Permite cálculo automático da idade, essencial para análise demográfica do corpo médico, verificação de aposentadoria e planejamento de sucessão profissional.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>tipo</strong></td>
    <td style="text-align: center;">Classificação do médico (M0, M1, M2)</td>
    <td style="text-align: center;">Indica o nível hierárquico ou tipo de contratação do médico, o que determina responsabilidades, remuneração e escopo de atuação.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>especialidades</strong></td>
    <td style="text-align: center;">Array de códigos de especialidades médicas</td>
    <td style="text-align: center;">Define as áreas de atuação do médico, permitindo direcionar pacientes de acordo com suas necessidades específicas, organizar escalas de plantão e distribuir casos adequadamente.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>contato.telefone</strong></td>
    <td style="text-align: center;">Número de telefone com DDD</td>
    <td style="text-align: center;">Permite contato direto em situações de emergência, alterações de escala ou comunicações urgentes sobre pacientes.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>contato.email</strong></td>
    <td style="text-align: center;">Endereço de e-mail</td>
    <td style="text-align: center;">Canal de comunicação formal para envio de relatórios, notificações administrativas, atualizações de protocolos e agendamentos.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>status</strong></td>
    <td style="text-align: center;">Situação atual do médico (Ativo/Inativo)</td>
    <td style="text-align: center;">Indica se o profissional está disponível para atendimentos ou temporariamente/permanentemente afastado, permitindo gestão adequada de recursos humanos.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>em_atividade</strong></td>
    <td style="text-align: center;">Status atual de serviço (booleano)</td>
    <td style="text-align: center;">Flag que indica se o médico está trabalhando no momento (em plantão ou expediente). Permite rastreamento em tempo real para encaminhamentos urgentes e gestão de escala.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>fila_de_pacientes</strong></td>
    <td style="text-align: center;">Lista de IDs de pacientes aguardando</td>
    <td style="text-align: center;">Controla pacientes na fila de espera do médico, essencial para organização do fluxo de atendimento e gestão de tempo. Permite priorização e redistribuição quando necessário.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.cpf</strong></td>
    <td style="text-align: center;">Cadastro de Pessoa Física</td>
    <td style="text-align: center;">Identificador fiscal necessário para processos administrativos, folha de pagamento, emissão de notas fiscais e declarações tributárias.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.crm</strong></td>
    <td style="text-align: center;">Registro no Conselho Regional de Medicina</td>
    <td style="text-align: center;">Documento legal obrigatório que comprova habilitação profissional. O prefixo "SP" indica o estado de registro, essencial para validação da autorização para exercício da medicina.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_consultas</strong></td>
    <td style="text-align: center;">Lista de identificadores de consultas</td>
    <td style="text-align: center;">Registra o histórico de atendimentos realizados pelo médico, permitindo análise de produtividade, distribuição de carga de trabalho e acesso rápido ao histórico de casos atendidos.</td>
  </tr>
</table>

# Tipos e Especialidades

<div style="display: flex; justify-content: center; width: 100%;">
    <div style="width: 50%; padding: 10px;">
        <!-- Tabela de Pacientes -->
       <table align="center" style="text-align: center;" style="width: 100%">
<tr>
<th width="30%" style="text-align: center;" >Tipo</th>
<th width="70%" style="text-align: center;" >Descrição</th>
</tr>
<tr>
<td style="text-align: center;">M0</td>
<td style="text-align: center;">Clínico Geral</td>
</tr>
<tr>
<td style="text-align: center;">M1</td>
<td style="text-align: center;">Dermatologista</td>
</tr>
<tr>
<td style="text-align: center;">M2</td>
<td style="text-align: center;">Pediatra</td>
</tr>
<tr>
<td style="text-align: center;">M3</td>
<td style="text-align: center;">Ginecologista</td>
</tr>
<tr>
<td style="text-align: center;">M4</td>
<td style="text-align: center;">Cirurgião</td>
</tr>
<tr>
<td style="text-align: center;">M5</td>
<td style="text-align: center;">Oftalmologista</td>
</tr>
</table>
    </div>
     <div style="width: 50%; padding: 10px;">
            <table align="center" style="text-align: center;" style="width: 100%">
<tr>
<th width="30%" style="text-align: center;" >Especialidade</th>
<th width="70%" style="text-align: center;" >Descrição</th>
</tr>
<tr>
<td style="text-align: center;">A</td>
<td style="text-align: center;">Dermatologia</td>
</tr>
<tr>
<td style="text-align: center;">B</td>
<td style="text-align: center;">Pediatria</td>
</tr>
<tr>
<td style="text-align: center;">C</td>
<td style="text-align: center;">Urologia</td>
</tr>
<tr>
<td style="text-align: center;">D</td>
<td style="text-align: center;">Oftalmologia</td>
</tr>
<tr>
<td style="text-align: center;">E</td>
<td style="text-align: center;">Neurologia</td>
</tr>
<tr>
<td style="text-align: center;">F</td>
<td style="text-align: center;">Cardiologia</td>
</tr>
</table>

  </div>
</div>
</div>