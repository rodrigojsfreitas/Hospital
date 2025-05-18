<div align="center">
      <img src="https://img.icons8.com/color/48/000000/nurse-female.png" width="200"/>

# Enfermeiras
      
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
    <td style="text-align: center;"><strong>uuid_enfermeira</strong></td>
    <td style="text-align: center;">Identificador único universal</td>
    <td style="text-align: center;">Garante identificação única da enfermeira no sistema e entre diferentes sistemas, prevenindo duplicações mesmo em ambientes distribuídos. Segue o formato padrão UUID.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_medico</strong></td>
    <td style="text-align: center;">Código alfanumérico simplificado</td>
    <td style="text-align: center;">Apesar do nome "id_medico", este campo serve como identificador interno da enfermeira. O prefixo "enf" seguido pelo estado ("sp") e número sequencial permite identificação rápida no dia a dia hospitalar.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>nome</strong></td>
    <td style="text-align: center;">Nome completo da enfermeira</td>
    <td style="text-align: center;">Identificação primária usada em todas as interações com pacientes, documentos oficiais, escalas de trabalho e comunicações institucionais.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>data_nascimento</strong></td>
    <td style="text-align: center;">Data de nascimento no formato ISO</td>
    <td style="text-align: center;">Permite cálculo automático da idade, essencial para análise demográfica do corpo de enfermagem, verificação de aposentadoria e planejamento de recursos humanos.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>tipo</strong></td>
    <td style="text-align: center;">Classificação da enfermeira (E0, E1, E2)</td>
    <td style="text-align: center;">Indica o nível hierárquico ou tipo de especialização da enfermeira, o que determina responsabilidades, remuneração e escopo de atuação.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>especialidades</strong></td>
    <td style="text-align: center;">Array de códigos de especialidades de enfermagem</td>
    <td style="text-align: center;">Define as áreas de atuação e competências específicas da enfermeira, permitindo alocação adequada conforme necessidades dos setores, organização de escalas e atendimento especializado aos pacientes.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>contato.telefone</strong></td>
    <td style="text-align: center;">Número de telefone</td>
    <td style="text-align: center;">Permite contato direto em situações de emergência, alterações de escala ou comunicações urgentes sobre pacientes. Fundamental para gestão de plantões e convocações extraordinárias.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>contato.email</strong></td>
    <td style="text-align: center;">Endereço de e-mail</td>
    <td style="text-align: center;">Canal de comunicação formal para envio de relatórios, comunicados administrativos, atualizações de protocolos, agendamentos e materiais de capacitação continuada.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>status</strong></td>
    <td style="text-align: center;">Situação atual da enfermeira (Ativo/Inativo)</td>
    <td style="text-align: center;">Indica se a profissional está disponível para atendimentos ou temporariamente/permanentemente afastada, permitindo gestão adequada de recursos humanos e planejamento de escalas.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.cpf</strong></td>
    <td style="text-align: center;">Cadastro de Pessoa Física</td>
    <td style="text-align: center;">Identificador fiscal necessário para processos administrativos, folha de pagamento, emissão de notas fiscais e declarações tributárias. Documento de verificação obrigatória para contratação.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.coren</strong></td>
    <td style="text-align: center;">Registro no Conselho Regional de Enfermagem</td>
    <td style="text-align: center;">Documento legal obrigatório que comprova habilitação profissional. O prefixo "SP" indica o estado de registro, essencial para validação da autorização para exercício da enfermagem e verificação de regularidade profissional.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>em_atividade</strong></td>
    <td style="text-align: center;">Status atual de serviço (booleano)</td>
    <td style="text-align: center;">Flag que indica se a enfermeira está trabalhando no momento (em plantão ou expediente). Permite rastreamento em tempo real para alocação de tarefas, distribuição de pacientes e gestão de ocorrências.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>fila_de_pacientes</strong></td>
    <td style="text-align: center;">Lista de IDs de pacientes sob responsabilidade</td>
    <td style="text-align: center;">Controla pacientes alocados ou atribuídos à enfermeira durante seu turno, essencial para organização do fluxo de atendimento, distribuição equilibrada de carga de trabalho e continuidade do cuidado.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_consultas</strong></td>
    <td style="text-align: center;">Lista de identificadores de consultas</td>
    <td style="text-align: center;">Registra o histórico de atendimentos e procedimentos nos quais a enfermeira participou, permitindo análise de produtividade, rastreabilidade de eventos adversos e responsabilização por procedimentos realizados.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_pacientes</strong></td>
    <td style="text-align: center;">Lista de identificadores de pacientes</td>
    <td style="text-align: center;">Relaciona os pacientes que foram ou estão sendo atendidos pela enfermeira, facilitando a continuidade do cuidado, acesso rápido ao histórico de interações e análise da distribuição de pacientes entre a equipe de enfermagem.</td>
  </tr>
</table>
</div>
<div align="center">

# Tipos e Especialidades

</div>
<div style="display: flex; justify-content: center; width: 100%;">
    <div style="width: 50%; padding: 10px;">
        <!-- Tabela de Pacientes -->
       <table align="center" style="text-align: center;" style="width: 100%">
<tr>
<th width="30%" style="text-align: center;" >Tipo</th>
<th width="70%" style="text-align: center;" >Descrição</th>
</tr>
<tr>
<td style="text-align: center;">E0</td>
<td style="text-align: center;">Auxiliar de Enfermagem</td>
</tr>
<tr>
<td style="text-align: center;">E1</td>
<td style="text-align: center;">Técnica de Enfermagem</td>
</tr>
<tr>
<td style="text-align: center;">E2</td>
<td style="text-align: center;">Enfermeira</td>
</tr>
<tr>
</table>
    </div>
     <div style="width: 50%; padding: 10px;">
            <table align="center" style="text-align: center;" style="width: 100%">
<tr>
<th width="30%" style="text-align: center;" >Especialidade</th>
<th width="70%" style="text-align: center;" >Descrição</th>
</tr>
<tr>
<td style="text-align: center;">G</td>
<td style="text-align: center;">Enfermagem Geriátrica</td>
</tr>
<tr>
<td style="text-align: center;">H</td>
<td style="text-align: center;">Enfermagem Ginecológica</td>
</tr>
<tr>
<td style="text-align: center;">I</td>
<td style="text-align: center;">Enfermagem Pediátrica</td>
</tr>
<tr>
<td style="text-align: center;">J</td>
<td style="text-align: center;">Enfermagem de Urgência</td>
</tr>
<tr>
<td style="text-align: center;">K</td>
<td style="text-align: center;">Enfermagem Cardiológica</td>
</tr>
<tr>
<td style="text-align: center;">L</td>
<td style="text-align: center;">Enfermagem Dermatológica</td>
</tr>
</table>

  </div>
</div>
</div>
