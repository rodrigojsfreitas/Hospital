 <div align="center">
      <img src="https://img.icons8.com/color/48/000000/pills.png" width="200"/>

# Estoque

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
    <td style="text-align: center;"><strong>id_medicamento</strong></td>
    <td style="text-align: center;">Identificador único do medicamento</td>
    <td style="text-align: center;">Permite rastreamento preciso de cada item no estoque, facilitando inventário, dispensação e integração com sistemas de prescrição. O formato alfanumérico (ex: "fhai3123") garante unicidade mesmo em grandes bases de dados farmacêuticos.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>medicamento</strong></td>
    <td style="text-align: center;">Nome do produto farmacêutico</td>
    <td style="text-align: center;">Identifica o medicamento de forma compreensível para humanos, sendo essencial para comunicação clara entre profissionais de saúde e para verificação visual durante dispensação, reduzindo erros de medicação.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>tipo_receita</strong></td>
    <td style="text-align: center;">Classificação do tipo de prescrição necessária</td>
    <td style="text-align: center;">Define os requisitos legais para dispensação (comum ou controlada), determinando procedimentos específicos de armazenamento, dispensação e controle. Impacta diretamente na segurança e conformidade regulatória da farmácia hospitalar.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>dosagem</strong></td>
    <td style="text-align: center;">Concentração do princípio ativo por unidade</td>
    <td style="text-align: center;">Especifica a quantidade exata de substância ativa presente em cada forma farmacêutica, informação crucial para cálculos de posologia, ajustes de dose e prevenção de erros de medicação, especialmente em populações vulneráveis.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>tarja</strong></td>
    <td style="text-align: center;">Classificação visual de segurança</td>
    <td style="text-align: center;">Categoriza o medicamento conforme potencial de risco (Amarela, Vermelha, Preta), sinalizando visualmente o nível de controle necessário. Essencial para organização física do estoque, alertas em sistemas eletrônicos e conformidade com normas sanitárias.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>restricoes</strong></td>
    <td style="text-align: center;">Limitações e cuidados especiais</td>
    <td style="text-align: center;">Detalha condições específicas para uso do medicamento, como necessidade de prescrição, restrições etárias ou ambientais. Fundamental para segurança do paciente, orientação adequada no momento da dispensação e prevenção de uso inadequado.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>via</strong></td>
    <td style="text-align: center;">Método de administração</td>
    <td style="text-align: center;">Define como o medicamento deve ser administrado (oral, intravenosa, intramuscular, retal), determinando aspectos críticos como biodisponibilidade, início de ação e riscos associados à administração. Imprescindível para prevenção de erros graves na aplicação.</td>
  </tr>
  <tr>
    <td style="text-align: center;"><strong>dosagem_maxima</strong></td>
    <td style="text-align: center;">Limite diário máximo permitido</td>
    <td style="text-align: center;">Estabelece o teto de segurança para administração diária total, servindo como parâmetro para sistemas de alerta que previnem sobredosagem e efeitos tóxicos. Especialmente crítico para medicamentos de baixo índice terapêutico ou potencialmente letais em overdose.</td>
  </tr>
</table>
</div>