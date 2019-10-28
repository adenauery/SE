
# Sistemas Embarcados

### 05/08/2019
* Introdução à disciplina
* Discussão do artigo: Elicitação e Especificação de Requisitos em Sistemas Embarcados: Uma Revisão Sistemática
* Definição inicial dos projetos a serem desenvolvidos

### 12/08/2019
* Avançar na discussão do esforço de especificação de requisitos em Sistemas Embarcados
* [Metodologia de Desenvolvimento de Sistemas Embarcados](https://pt.slideshare.net/AlexandreAugustoGiron/metodologias-de-desenvolvimento-de-sistemas-embarcados)
* Discussão do artigo: [TERASE: Template para Especificação de Requisitos de Ambiente em Sistemas Embarcados](http://wer.inf.puc-rio.br/WERpapers/artigos/artigos_WER10/martins.pdf)
* Definição dos projetos a serem desenvolvidos

### 19/08/2019
* Discussão do artigo: [GERSE: Guia de Elicitação de Requisitos para Sistemas Embarcados](http://www.inf.puc-rio.br/wer/WERpapers/artigos/artigos_WER12/paper_3.pdf)
* [Elicitação e Especificação de Requisitos para Sistemas Embarcados - Comparação TERASE & GERSE](https://www.cin.ufpe.br/~in1020/previous/2016.2/docs/works/inicial/Work_Reinaldo.pdf)
* Definição dos projetos a serem desenvolvidos

### 26/08/2019
* Definição do escopo dos projetos
* Início do preenchimento da Tabela GERSE do projeto
* Especificação inicial do hardware/software a ser utilizado

### 02/09/2019
* Conclusão da definição dos escopos do projeto
* Avanço no preenchimento da tabela GERSE
* Continuidade da especificação do hardware/software envolvido

### 09/09/2019
* Revisão da tabela GERSE
* [Quick Sequence Diagram Editor - Diagrama de Sequencia editado em modo texto](https://sourceforge.net/projects/sdedit/)
* [Draw.io - Diagramas UML (portanto Sequência também) em modo gráfico](https://www.draw.io/)
* Modelo Arquitetural empregando o GoogleDocs (Apresentação)

### 16/09/2019
* Finalização da Tabela GERSE caracterizando os esforços necessários para os diferentes projetos

### 23/09/2019
* Escrita dos Resumos dos projetos da turma
* Revisão dos esforços de prototipação

### 30/09/2019
* Revisão dos Resumos de todos os projetos da turma
* Iniciar a construção dos Diagramas de Sequência do UML referentes aos projetos
  * Considerar o uso das ferramentas: [Quick Sequence Diagram Editor](https://sourceforge.net/projects/sdedit/) e [PlantUML](http://plantuml.com/sequence-diagram)
  
### 07/10/2019
 * Revisão dos procedimentos de implementação referentes ao protótipo em desenvolvimento
 * Revisão da construção dos Diagramas de Sequencia em UML dos projetos
 
### 14/10/2019
 * Recesso Academico e Administrativo da UCPEL
 
### 21/10/2019
 * Ajustes nas metas mecânicas & eletrônicas dos projetos, considerando sua viabilidade no semestre em andamento
 
### 28/10/2019
 * **Cronograma de Atividades até o final do semestre
   * 02/12 - Demonstração prática do Projeto
   * 09/12 - Apresentação do Projeto, e entrega do Relatório Final
 
 * **Composição do Relatório Final
   * Capa: com título e indicação do autor
   * Resumo: que traduza os aspectos mais importantes
   * [1] Introdução: compreendendo a motivação, objetivo geral e objetivos específicos
   * [2] Tabela Gerse do Projeto
   * [3] Descrição do Hardware utilizado: podem ser utilizadas fotos, etc.
   * [4] Descrição do Software: empregando diagramas UML combinados com trechos de texto. Também podem ser utilizados fluxogramas para descrição dos softwares
   * [5] Operação do Projeto: caracterização de como o Projeto acontece, com registro das diferentes operações e as respectivas interfaces tanto de hardware como de software
   * [6] Considerações finais
   * Referências bibliográficas
   
 * **Modelo de Relatório
   * O colega Victor Hugo Lima organizou um modelo de Relatório Final. Vide abaixo:
   * [Link somente leitura no Overleaf](https://www.overleaf.com/read/frqrqpvnntdy)

## Links Relativos à Disciplina:

* [Disciplina "Sistemas Embarcados" na UFPEL](https://institucional.ufpel.edu.br/disciplinas/cod/1110070)
* [Robot Operating System](https://www.ros.org/)
* https://www.embarcados.com.br/sistemas-embarcados-e-microcontroladores/
* https://www.embarcados.com.br/icarus-iot-board/
* Tutoriais sobre o Git:
  * https://rogerdudler.github.io/git-guide/index.pt_BR.html
  * https://www.hostinger.com.br/tutoriais/comandos-basicos-de-git/
* Livro sobre o Git
  * [Pro Git book, Scott Chacon and Ben Straub](https://git-scm.com/book/pt-br/v2)
* Resetando a ESP3
```
  import sys
  import machine
  import network
  sta_if = network.WLAN(network.STA_IF)
  sta_if.active(False)
  ap_if = network.WLAN(network.AP_IF)
  ap_if.active(False)
  sys.exit()
  machine.reset()
```

## Projetos da Turma

**Karen Rediess Müller**
* Spin Coater: Uma Abordagem para Controle pela IoT
* [GitHub do Projeto](https://github.com/KarencomK/SistemasEmbarcados)
  * https://lista.mercadolivre.com.br/ethernet-shield-w5100#D
  * https://www.caldeiratech.com/arduinos/kit-arduino-mega-2560-ethernet-shield-w5100-c-slot-sd-card/

**Lucas Pereira Ferreira**
* QR-Nefro: Controle de Pacientes em um Serviço de Nefrologia
* [GitHub do Projeto](https://github.com/lucaspeferreira/qr-nefro/issues/)

**Matheus Kern Protzen**
* iArm: um Braço Mecânico Controlado pela Internet
* [GitHub do Projeto](https://github.com/MatheusKProt/braco_mecanico)
* [Robot Operating System](https://www.ros.org/)

**Thayná Almeida da Rosa de Oliveira**
* iMid: Um Middleware para Atualização de Códigos Python pela IoT
* [GitHub do Projeto](https://github.com/euthayna/)
  * Sensores: 
    * temperatura: DS18b20 
    * luminosidade: LDR

**Victor Hugo da Silveira Lima**
* sLock: Fechadura Inteligente com Registro de Operação e Controle pela Internet
* [GitHub do Projeto](https://github.com/Victorhlima98/Fechadura_Inteligente)
