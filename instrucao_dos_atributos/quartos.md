   <div align="center">
      <img src="https://img.icons8.com/color/48/000000/hospital-bed.png" width="200"/>

# Quarto

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
    <td align="center"><strong>id_quarto</strong></td>
    <td align="center">Identificador único do quarto</td>
    <td align="center">Permite referência única a cada quarto no sistema hospitalar, facilitando busca, alocação e integração com outros módulos como internação e faturamento. O formato padronizado (Q101) combina letra e número para distinção clara na comunicação verbal e escrita.</td>
  </tr>
  <tr>
    <td align="center"><strong>numero</strong></td>
    <td align="center">Número físico do quarto</td>
    <td align="center">Corresponde à numeração real na sinalização do hospital, facilitando a localização física por pacientes, visitantes e profissionais. Essencial para orientação dentro da estrutura hospitalar e planejamento logístico.</td>
  </tr>
  <tr>
    <td align="center"><strong>ala</strong></td>
    <td align="center">Setor do hospital</td>
    <td align="center">Define a especialidade ou finalidade da unidade (Enfermaria, UTI, Maternidade), determinando recursos disponíveis, protocolos aplicáveis e equipe responsável. Permite gestão setorizada e direcionamento adequado de pacientes conforme necessidades clínicas.</td>
  </tr>
  <tr>
    <td align="center"><strong>tipo</strong></td>
    <td align="center">Configuração do quarto</td>
    <td align="center">Classifica o quarto quanto à privacidade e distribuição (Individual, Duplo, Coletivo), influenciando diretamente fatores como faturamento, controle de infecção hospitalar, disponibilidade para acompanhantes e adequação a diferentes convênios médicos.</td>
  </tr>
  <tr>
    <td align="center"><strong>capacidade</strong></td>
    <td align="center">Número máximo de leitos</td>
    <td align="center">Estabelece o limite de pacientes que podem ocupar simultaneamente o quarto, crucial para gestão de ocupação, planejamento de internações e dimensionamento de recursos assistenciais para cada espaço físico.</td>
  </tr>
  <tr>
    <td align="center"><strong>Disponível</strong></td>
    <td align="center">Status de ocupação (booleano)</td>
    <td align="center">Indica em tempo real se o quarto pode receber novos pacientes, permitindo decisões rápidas sobre admissões, transferências e planejamento de altas. Essencial para gestão de leitos, especialmente em situações de alta demanda.</td>
  </tr>
  <tr>
    <td align="center"><strong>equipamentos</strong></td>
    <td align="center">Lista de dispositivos disponíveis</td>
    <td align="center">Documenta recursos técnicos permanentes do quarto (Monitor cardíaco, Oxigênio, Respirador), permitindo alocação adequada de pacientes conforme necessidades clínicas, preparação prévia para recepção e planejamento de manutenções preventivas.</td>
  </tr>
  <tr>
    <td align="center"><strong>responsaveis</strong></td>
    <td align="center">IDs dos profissionais designados</td>
    <td align="center">Vincula o quarto às equipes médica e de enfermagem responsáveis, estabelecendo responsabilidade assistencial, facilitando comunicação em emergências e permitindo análise de distribuição de carga de trabalho entre profissionais.</td>
  </tr>
  <tr>
    <td align="center"><strong>limpeza_status</strong></td>
    <td align="center">Estado atual de higienização</td>
    <td align="center">Indica se o quarto está "Limpo" ou "Sujo", essencial para controle de infecção hospitalar, liberação para novas ocupações e planejamento da equipe de higienização. Impacta diretamente na segurança do paciente e na velocidade de rotatividade dos leitos.</td>
  </tr>
  <tr>
    <td align="center"><strong>ultima_limpeza</strong></td>
    <td align="center">Data e hora da última higienização</td>
    <td align="center">Registra quando o quarto foi limpo pela última vez, permitindo auditoria de processos, planejamento de limpezas terminais periódicas e verificação de conformidade com protocolos de controle de infecção hospitalar.</td>
  </tr>
  <tr>
    <td align="center"><strong>pacientes_ocupantes</strong></td>
    <td align="center">Array com dados dos pacientes atuais</td>
    <td align="center">Documenta quem está ocupando o quarto no momento, incluindo identificação e cronologia (entrada/saída). Permite gestão em tempo real da ocupação, faturamento preciso do período e rastreabilidade em investigações epidemiológicas de infecções hospitalares.</td>
  </tr>
  <tr>
    <td align="center"><strong>historico_ocupacao</strong></td>
    <td align="center">Registro de ocupações anteriores</td>
    <td align="center">Mantém o histórico completo de todos os pacientes que ocuparam o quarto, essencial para investigações epidemiológicas retroativas, auditoria de ocupação, análise de taxas de reocupação e estudos de eficiência operacional do hospital.</td>
  </tr>
  <tr>
    <td align="center"><strong>ultima_visita</strong></td>
    <td align="center">Dados da última avaliação médica</td>
    <td align="center">Registra informações sobre a visita médica mais recente ao quarto, incluindo profissional, momento e observações clínicas. Facilita continuidade assistencial entre turnos, documentação de condutas e monitoramento da frequência de acompanhamento médico.</td>
  </tr>
</table>
</div>