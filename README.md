<div align="center">
  
  # 🏥 Hospital - Banco de Dados NoSQL
  
  <!-- Enhanced Banner with More Colors -->
  <img src="https://img.shields.io/badge/🏥_HOSPITAL_DB-SYSTEM-E91E63?style=for-the-badge" alt="Hospital DB" />
  <br>
    
  ![](https://img.shields.io/badge/Database-NoSQL-00C4CC?style=for-the-badge&logo=mongodb&logoColor=white)
  ![](https://img.shields.io/badge/Format-JSON-F7DF1E?style=for-the-badge&logo=json&logoColor=black)
  ![](https://img.shields.io/badge/Last_Updated-May_2025-FF5722?style=for-the-badge)

</div>

---

<!-- ANIMATED TOC SECTION with Enhanced Colors -->
<details open>
<summary><b>📑 NAVEGAÇÃO RÁPIDA</b></summary>


| 📑 |<div align="center"> Seção  </div>             | 📑 | <div align="center"> Seção  </div>                 |
|:-:|:--------------------|:-:|:-----------------------|
| 🔍 | <div align="center"> [<span style="color:#3F51B5">Visão Geral</span>](#-visão-geral) </div> | 🎯 | <div align="center">[<span style="color:#E91E63">Objetivos</span>](#-objetivos) </div>|
| 📊 | <div align="center">[<span style="color:#00C4CC">Estrutura</span>](#-estrutura-de-dados)</div> | 🚀 | <div align="center">[<span style="color:#FF9800">Casos de Uso</span>](#-casos-de-uso)</div> |
| 🔄 | <div align="center">[<span style="color:#4CAF50">Arquitetura</span>](#-arquitetura)</div> | 📋 | <div align="center">[<span style="color:#9C27B0">Instruções</span>](#-instruções-da-atividade)</div> |
| 💻 | <div align="center">[<span style="color:#2196F3">Tecnologias</span>](#-tecnologias)</div> | ⚠️ |<div align="center"> [<span style="color:#F44336">Aviso</span>](#%EF%B8%8F-aviso) </div>|
</details>

---

<!-- MAIN CONTENT with Enhanced Colors -->
## 🔍 <span style="color:#3F51B5">VISÃO GERAL</span>

<img align="right" width="150" src="https://img.icons8.com/color/240/000000/hospital-3.png" />

> **Bem-vindo ao projeto Hospital!**

Este sistema representa uma **revolucionária** abordagem à gestão de dados hospitalares utilizando arquitetura **NoSQL** para maior flexibilidade, escalabilidade e performance.

`Por que NoSQL para hospitais?` Ambientes de saúde exigem estruturas de dados flexíveis que possam se adaptar rapidamente a diferentes:
* 🧑‍⚕️ Tipos de pacientes e condições
* 📋 Protocolos médicos em evolução
* 📜 Requisitos regulatórios em constante mudança
* 🔄 Integração com diversos sistemas eletrônicos

<br>

## 📊 <span style="color:#00C4CC">ESTRUTURA DE DADOS</span>

Nossa base de dados é organizada em documentos JSON, cada um representando uma entidade crítica no ecossistema hospitalar:

<table>
<tr style="background-color:#E3F2FD">
  <th width="25%">Documento</th>
  <th width="35%">Descrição</th>
  <th width="40%">Atributos</th>
</tr>
<tr style="background-color:#F3E5F5">
  <td>
    <a href="./hospital_DB/pacientes.json"><img src="https://img.shields.io/badge/_pacientes.json-3F51B5?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Paciente.json"/></a>
       <!-- <img src="https://img.icons8.com/?size=100&id=14874&format=png&color=000000" width="54"/> Paciente.json -->
  </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/?size=100&id=14874&format=png&color=000000" width="54"/><br>
      
  <a href="./instrucao_dos_atributos/pacientes.md">Cadastro completo de pacientes</a>
    </div></td>
  <td align="center">
    <code>uuid_paciente</code>, <code>id_paciente</code>, <code>nome</code>, <code>data_nascimento</code>, <code>documentos (CPF, RG, etc)</code>, <code>contato</code>, <code>endereco</code>, <code>tipo_sanguineo</code>, <code>convenio</code>, <code>prontuario</code>, <code>id_receitas[]</code></td>
</tr>
<tr style="background-color:#E8F5E9">
  <td>
       <!-- <img src="https://img.icons8.com/color/48/000000/doctor-male.png" width="24"/> Médico.json -->
       <a href="./hospital_DB/medicos.json"><img src="https://img.shields.io/badge/medicos.json-388E3C?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Médico.json"/></a>
  </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/color/48/000000/doctor-male.png" width="54"/>
      <br>  
  <a href="./instrucao_dos_atributos/medicos.md">Perfil dos médicos e especialidades</a></div></td>
  <td align="center">
<code>uuid_medico</code>, <code>id_medico</code>, <code>nome</code>, <code>data_nascimento</code>, <code>tipo</code>, <code>especialidades[]</code>, <code>contato</code>, <code>status</code>, <code>em_atividade</code>, <code>fila_de_pacientes[]</code>, <code>documentos (CPF e CRM)</code>, <code>id_consultas[]</code>, <code>id_pacientes[]</code></td>
</tr>
<tr style="background-color:#FFF3E0">
  <td><!--<img src="https://img.icons8.com/color/48/000000/nurse-female.png" width="24"/> <b> Enfermeira.json</b>-->
      <a href="./hospital_DB/enfermeiras.json"><img src="https://img.shields.io/badge/enfermeiras.json-FF9800?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Enfermeira.json"/></a>
  
  </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/color/48/000000/nurse-female.png" width="54"/> 
      <br>
    <a href="./instrucao_dos_atributos/enfermeiras.md">Equipe de enfermagem e atribuições</a></div></td>
  <td align="center">
    <code>uuid_enfermeira</code>, <code>id_medico</code>, <code>nome</code>, <code>data_nascimento</code>, <code>tipo</code>, <code>especialidades[]</code>, <code>contato</code>, <code>status</code>, <code>documentos (COREN e CPF)</code>, <code>em_atividade</code>, <code>fila_de_pacientes[]</code>, <code>id_consultas[]</code>, <code>id_pacientes[]</code></tr>
<tr style="background-color:#E0F7FA">
  <td><!--<img src="https://img.icons8.com/color/48/000000/health-checkup.png" width="24"/> <b> Consulta.json</b>-->
      <a href="./hospital_DB/consultas.json"><img src="https://img.shields.io/badge/consultas.json-00BCD4?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Consulta.json"/></a>
  
  </td>
  <td>
  <div align="center">
    <img src="https://img.icons8.com/color/48/000000/health-checkup.png" width="54"/>
    <br>
    
  <a href="./instrucao_dos_atributos/consultas.md">Histórico de atendimentos médicos</a> </div></td>
  <td align="center">
    <code>id_consulta</code>, <code>id_paciente</code>, <code>id_responsavel[]</code>, <code>especialidade</code>, <code>data_entrada</code>, <code>data_prevista_entrada</code>, <code>data_prevista_saida</code>, <code>data_saida</code></td>
</tr>
<tr style="background-color:#F1F8E9">
  <td><!--<img src="https://img.icons8.com/color/48/000000/microscope.png" width="24"/> <b> Exames.json</b> -->
  <a href="./hospital_DB/exames.json"><img src="https://img.shields.io/badge/exames.json-8BC34A?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Exames.json"/></a>
      
  </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/color/48/000000/microscope.png" width="54"/> <br>
      
  <a href="./instrucao_dos_atributos/exames.md">Procedimentos e diagnósticos</a></div></td>
  <td align="center">
 <code>paciente_id</code>, <code>id_responsavel</code>, <code>data_entrada</code>, <code>data_prevista_alta</code>, <code>data_efetiva_alta</code>, <code>procedimentos (Procedimento, Exame)</code>, <code>quarto_id</code>, <code>id_dos_responsaveis[]</code>
  </td>
</tr>
<tr style="background-color:#FCE4EC">
  <td><!--<img src="https://img.icons8.com/?size=100&id=13HpMwhzW71Q&format=png&color=000000" width="24"/> <b> Receitas.json</b>-->
      <a href="./hospital_DB/receitas.json"><img src="https://img.shields.io/badge/Receitas.json-E91E63?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Receitas.json"/></a>
  </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/?size=100&id=13HpMwhzW71Q&format=png&color=000000" width="54"/> <br>
      
  <a href="./instrucao_dos_atributos/receitas.md">Prescrições de medicamentos</a></div></td>
  <td align="center">
<code>id_receita</code>, <code>nome_medico</code>, <code>documento (CRM)</code>, <code>nome_paciente</code>, <code>id_responsaveis</code>, <code>id_paciente</code>, <code>data_prescrição</code>, <code>data_validade</code>, <code>medicamentos[]</code>, <code>observacao</code>, <code>dispensação</code></td>
</tr>
<tr style="background-color:#FFF8E1">
  <td><!--<img src="https://img.icons8.com/color/48/000000/pills.png" width="24"/> <b> Estoque.json</b>-->
  <a href="./hospital_DB/estoque.json"><img src="https://img.shields.io/badge/estoque.json-FFC107?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Estoque.json"/>
      
  </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/color/48/000000/pills.png" width="54"/> <br>
      
  <a href="./instrucao_dos_atributos/estoque.md">Inventário farmacêutico</a></div></td>
  <td align="center">
    <code>id_medicamento</code>, <code>medicamento</code>, <code>tipo_receita</code>, <code>dosagem</code>, <code>tarja</code>, <code>restricoes</code>, <code>via</code>, <code>dosagem_maxima</code></td>
</tr>
<tr style="background-color:#E8EAF6">
  <td>
        <!-- <img src="https://img.icons8.com/color/48/000000/hospital-bed.png" width="20"/> Quarto.json -->
    <a href="./hospital_DB/quartos.json"><img src="https://img.shields.io/badge/quartos.json-3F51B5?style=for-the-badge&logo=json&logoColor=white" width="1000" alt="Quartos.json"/></a>
      </td>
  <td>
    <div align="center">
      <img src="https://img.icons8.com/color/48/000000/hospital-bed.png" width="54"/> <br>
      
  <a href="./instrucao_dos_atributos/quartos.md">Gestão de acomodações</a></div></td>
  <td align="center">
     <code>id_quarto</code>, <code>numero</code>, <code>ala</code>, <code>tipo</code>, <code>capacidade</code>, <code>Disponível</code>, <code>equipamentos</code>, <code>responsaveis</code>, <code>limpeza_status</code>, <code>ultima_limpeza</code>, <code>pacientes_ocupantes (id_paciente, data_entrada, data_saida)</code>, <code>historico_ocupacao (id_paciente, data_entrada, data_saida)</code>, <code>ultima_visita (id_medico, data_visita, observacoes)</code></td>
</tr>
</table>

<div align="center">
<i>Cada documento segue um esquema cuidadosamente projetado que equilibra flexibilidade com consistência de dados.</i>
</div>

## 🔄 <span style="color:#4CAF50">ARQUITETURA</span>

<div align="center">
<img src="./img/imageDiagrama.png" alt="Hospital Database System Architecture" width="700"/>
<br>
<p style="background-color:#E1F5FE;padding:10px;border-radius:5px;border-left:4px solid #03A9F4;">
<b>Diagrama Entidade-Relacionamento do Sistema Hospitalar</b><br>
<i>Visualização das relações entre as principais entidades do sistema</i>
</p>
</div>

<br>

## 💻 <span style="color:#2196F3">TECNOLOGIAS</span>
<div align="center">
<table>
<tr style="background-color:#E3F2FD">
  <td align="center" width="96" style="background-color:#00C4CC20;border-radius:8px;">
    <img src="https://img.icons8.com/color/48/000000/mongodb.png" width="48" height="48" alt="MongoDB" />
    <br>MongoDB
  </td>
  <td align="center" width="96" style="background-color:#F7DF1E20;border-radius:8px;">
    <img src="https://img.icons8.com/color/48/000000/json.png" width="48" height="48" alt="JSON" />
    <br>JSON
  </td>
  </tr>
</table>
</div>

## 🎯 <span style="color:#E91E63">OBJETIVOS</span>

<img align="right" width="200" src="https://img.icons8.com/color/240/000000/goal--v1.png"/>

Este projeto foi desenvolvido com os seguintes objetivos:

- 📚 <span style="color:#3F51B5"><b>Ferramenta Educacional</b></span>: Exemplo completo de design de banco de dados NoSQL
- 📋 <span style="color:#009688"><b>Modelo de Referência</b></span>: Demonstração de modelagem de dados não relacionais

A implementação foca em cenários práticos do mundo real, mantendo simplicidade para fins educacionais.

## 🚀 <span style="color:#FF9800">CASOS DE USO</span>

O sistema de banco de dados hospitalar suporta diversos cenários de gestão de saúde, incluindo:

<div style="display: flex; justify-content: space-between;">
<div width="48%">

### <span style="color:#4CAF50">Operações com Dados</span>
- ✅ Operações **CRUD** completas em registros de pacientes
- 👨‍⚕️ Gestão e alocação de equipe médica
- 📅 Agendamento e registro de consultas
- 💊 Controle de inventário de medicamentos

</div>
<div width="48%">

### <span style="color:#2196F3">Análises & Relatórios</span>
- 📈 Análise de histórico de atendimento
- 📊 Avaliação de resultados de tratamentos

</div>
</div>


<div style="background: linear-gradient(90deg, #FF9800, #F44336); padding: 2px; border-radius: 5px;">
<div style="background: white; padding: 15px; border-radius: 3px;">

### <span style="color:#E91E63">Benefícios para o Hospital</span>

- 🏆 <span style="color:#4CAF50">Maior eficiência</span> no gerenciamento de dados clínicos
- 🔄 <span style="color:#2196F3">Integração simplificada</span> com sistemas externos
- 🛡️ <span style="color:#FF9800">Melhor segurança</span> e rastreabilidade de informações

</div>
</div>

## 📋 <span style="color:#9C27B0">INSTRUÇÕES DA ATIVIDADE</span>

<br>

<div align="center" style="background: linear-gradient(45deg, #9C27B0, #3F51B5); padding: 2px; border-radius: 8px; margin: 20px 0;">
  <div style="background: white; padding: 10px; border-radius: 6px">
    <a href="./atividade.md">
      <img src="https://img.shields.io/badge/📝_Ver_Instruções_Detalhadas-4285F4?style=for-the-badge" alt="Instruções da Atividade"/>
    </a>
  </div>
</div>


## ⚠️ <span style="color:#F44336">AVISO</span>

<div style="border-left: 4px solid #F44336; background-color: #FFEBEE; padding: 15px; border-radius: 0 5px 5px 0;">
<b>IMPORTANTE</b>: Todos os dados contidos neste projeto são inteiramente fictícios e criados exclusivamente para fins educacionais. Qualquer semelhança com pessoas reais ou registros médicos reais é mera coincidência.
</div>

---

<br>

<div align="center" style="background: linear-gradient(to right, #E91E63, #9C27B0, #3F51B5, #2196F3, #00BCD4, #009688, #4CAF50, #8BC34A, #CDDC39, #FFEB3B, #FFC107, #FF9800, #FF5722); height: 5px; border-radius: 5px; margin: 30px 0;"></div>

<div align="center">
  <p>Desenvolvido com ❤️ pelo <span style="color:#E91E63">rodrigojsfreitas</span></p>
  <p>Última atualização: <span style="color:#009688">2025-05-14 12:23:24</span></p>
  
</div>