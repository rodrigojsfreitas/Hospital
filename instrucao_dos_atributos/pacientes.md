<div align="center">
<img src="https://img.icons8.com/?size=100&id=14874&format=png&color=000000" width="200"/></div>
<div align="center">

# Pacientes
---
</div>
<div align="center">
<table align="center" style="text-align: center;">
  <tr>
    <th style="text-align: center;">Atributo</th>
    <th style="text-align: center;">Descrição</th>
    <th style="text-align: center;">Motivo/Importância</th>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>uuid_paciente</strong></td>
    <td style="text-align: center;">Identificador único universal</td>
    <td style="text-align: center;">Garante identificação única do paciente em todo o sistema e eventuais integrações, evitando duplicações e confusões mesmo em ambientes distribuídos. Segue o formato padrão UUID v4.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_paciente</strong></td>
    <td style="text-align: center;">Identificador simplificado</td>
    <td style="text-align: center;">Facilita a referência ao paciente em comunicações verbais e formulários, sendo mais fácil de memorizar e anotar que o UUID.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>nome</strong></td>
    <td style="text-align: center;">Nome completo do paciente</td>
    <td style="text-align: center;">Identificação primária do paciente para comunicação direta, documentos e registros oficiais.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>data_nascimento</strong></td>
    <td style="text-align: center;">Data de nascimento no formato ISO</td>
    <td style="text-align: center;">Permite cálculo automático da idade, auxilia na identificação de pacientes homônimos, e é crucial para definir dosagens medicamentosas e protocolos adequados por faixa etária.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.rg</strong></td>
    <td style="text-align: center;">Número do Registro Geral</td>
    <td style="text-align: center;">Documento oficial de identificação necessário para procedimentos administrativos e internações.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.digito</strong></td>
    <td style="text-align: center;">Dígito verificador do RG</td>
    <td style="text-align: center;">Complementa o RG, garantindo sua validação completa em verificações de identidade.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.cartaoSus</strong></td>
    <td style="text-align: center;">Número do Cartão Nacional de Saúde</td>
    <td style="text-align: center;">Permite acesso aos serviços do SUS e rastreamento de atendimentos na rede pública, fundamental para integração com o sistema nacional de saúde.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.cartaoClube</strong></td>
    <td style="text-align: center;">Cartão de benefícios do hospital</td>
    <td style="text-align: center;">Identifica associação a programas de fidelidade ou benefícios específicos oferecidos pela instituição.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>documentos.cpf</strong></td>
    <td style="text-align: center;">Cadastro de Pessoa Física</td>
    <td style="text-align: center;">Identificador fiscal necessário para processos administrativos, faturamento e emissão de notas fiscais.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>contato.subcontatoX.telefone</strong></td>
    <td style="text-align: center;">Número de telefone com DDD</td>
    <td style="text-align: center;">Canal primário para comunicação com o paciente para confirmações de consultas, resultados de exames e contatos emergenciais.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>contato.subcontatoX.whatsapp</strong></td>
    <td style="text-align: center;">Indicador se o número tem WhatsApp</td>
    <td style="text-align: center;">Permite envio de comunicações digitais como lembretes, orientações e receitas via aplicativo, reduzindo custos de comunicação.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.cep</strong></td>
    <td style="text-align: center;">Código de Endereçamento Postal</td>
    <td style="text-align: center;">Facilita a validação e autopreenchimento de endereço, reduzindo erros de cadastro e permitindo análises geográficas.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.logradouro</strong></td>
    <td style="text-align: center;">Nome da via (rua, avenida, etc.)</td>
    <td style="text-align: center;">Componente essencial do endereço para correspondências e visitas domiciliares quando necessário.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.numero</strong></td>
    <td style="text-align: center;">Número do imóvel</td>
    <td style="text-align: center;">Complemento necessário para localização exata do endereço.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.complemento</strong></td>
    <td style="text-align: center;">Informações adicionais do endereço</td>
    <td style="text-align: center;">Especifica detalhes como apartamento, bloco ou sala, essenciais para correspondências precisas.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.bairro</strong></td>
    <td style="text-align: center;">Bairro de residência</td>
    <td style="text-align: center;">Importante para regionalização de atendimentos e estudos epidemiológicos locais.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.cidade</strong></td>
    <td style="text-align: center;">Município de residência</td>
    <td style="text-align: center;">Essencial para encaminhamentos regionais e análise geográfica da distribuição de pacientes.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>endereco.estado</strong></td>
    <td style="text-align: center;">Unidade Federativa (UF)</td>
    <td style="text-align: center;">Complementa a informação geográfica para gestão de saúde pública e estatísticas.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>tipo_sanguineo</strong></td>
    <td style="text-align: center;">Tipo sanguíneo e fator RH</td>
    <td style="text-align: center;">Informação crítica para transfusões, procedimentos cirúrgicos e gestão do banco de sangue.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>convenio</strong></td>
    <td style="text-align: center;">Plano de saúde do paciente</td>
    <td style="text-align: center;">Define cobertura assistencial, processos de faturamento e autorizações necessárias para procedimentos.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>prontuario.AlergiaX</strong></td>
    <td style="text-align: center;">Registro de alergias</td>
    <td style="text-align: center;">Previne reações alérgicas a medicamentos, alimentos ou substâncias durante o tratamento, reduzindo riscos ao paciente.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>prontuario.DoencaX</strong></td>
    <td style="text-align: center;">Registro de doenças pré-existentes</td>
    <td style="text-align: center;">Influencia decisões de tratamento, precauções médicas e contraindica certas medicações, garantindo segurança no atendimento.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>id_receitas</strong></td>
    <td style="text-align: center;">Lista de identificadores de receitas</td>
    <td style="text-align: center;">Permite rastreamento do histórico medicamentoso, facilita renovações e controle de medicamentos de uso contínuo ou controlados.</td>
  </tr>
</table>
</div>