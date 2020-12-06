
# Sistemas Embarcados

### Equipe
|   |   |   |
|---|--:|:--|
| **Nome** |   |  | 
|Bruno Lopes Soares  | [Repositório](https://github.com/PoderosoBR/Esp32-MQTT) | [Projeto](https://github.com/PoderosoBR/Esp32-MQTT/wiki/Projeto-Esp32---Leitor-de-Dispositivos-para-Esp32) |
|Gustavo Ribeiro Iribarrem | [Repositório](https://github.com/iribarrem/SE) | [Projeto](https://github.com/iribarrem/SE/wiki) |
|Kaller Moraes Gonçalves | [Repositório](https://github.com/KallerMG/SE-esp32) |   [Projeto](https://github.com/KallerMG/Iot_jardim/wiki) |
|Lucas Kerstner Penning | [Repositório](https://github.com/lucaspenning/sistemas_embarcados) | [Projeto](https://github.com/lucaspenning/Telegram_OTA) |
|Wellington Weikamp Porto  |  [Repositório](https://github.com/wellkamp/sistemas_embarcados)| [Projeto](https://github.com/wellkamp/iot_cloud_br/blob/main/README.md) |
|   |   |   | |

--------- | ------ | ------
Aluno     | Valor do exemplo | Exemplo 2
Exemplo 1 | R$ 10  | 55
Exemplo 2 | R$ 8.  | 44
Exemplo 3 | R$ 7   | 33
Exemplo 4 | R$ 8   | 22

---

### Apresentações
|   |   |   |
|---|:--|:--|
| **Nome** | 1a Atividade  | 2a Atividade | 
|Bruno Lopes Soares  | 14/09  | 21/09 | 
|Gustavo Ribeiro Iribarrem |  | 21/09 |
|Kaller Moraes Gonçalves | 14/09 | 21/09 |
|Lucas Kerstner Penning | 14/09 | 21/09 |
|Wellington Weikamp Porto  | 14/09 | 21/09 |
|   |   |   |

### 27/07/2020
* Introdução à disciplina
  * Definição Embarcado a ser utilizado: ESP32
  * Atividades Iniciais de Programação com [MicroPython](http://olaria.ucpel.edu.br/micropython/)
  * Temas de interesse em pesquisa
  * [Capítulo de Livro Utilizado no Primeiro Encontro](https://meet.google.com/linkredirect?authuser=2&dest=https%3A%2F%2Fintegrada.minhabiblioteca.com.br%2F%23%2Fbooks%2F9788536520346%2Fpageid%2F21) - Disponível na Minha Biblioteca
* Discussão do artigo: [Elicitação e Especificação de Requisitos em Sistemas Embarcados: Uma Revisão Sistemática](https://pdfs.semanticscholar.org/59d1/09b7dce30ef4727279a8d32810c94278a115.pdf?_ga=2.56763946.1847345786.1595809313-1098268385.1595809313)

#### Atividades Não Síncronas
  * Gravando Dados Coletados em uma Plataforma de Nuvem
    * Registro histórico dos dados: [Exemplo](https://fazerlab.wordpress.com/2017/10/24/dados-em-tempo-real-com-planilha-do-google-docs/) 
    * Visualizando os dados: [Exemplo](https://fazerlab.wordpress.com/2017/10/30/grafico-dinamico-com-google-script-e-planilha/)

  * Google Apps Scripts.
    * [Apresentação](http://olaria.ucpel.edu.br/materiais/lib/exe/fetch.php?media=apresentacao-google-apps-script.pdf)
    * [Livro](http://olaria.ucpel.edu.br/materiais/lib/exe/fetch.php?media=livro-google-apps-script.pdf)

---

### 03/08/2020
* Avançar na discussão do esforço de especificação de requisitos em Sistemas Embarcados
* [Metodologia de Desenvolvimento de Sistemas Embarcados](https://pt.slideshare.net/AlexandreAugustoGiron/metodologias-de-desenvolvimento-de-sistemas-embarcados)
* Discussão do artigo: [TERASE: Template para Especificação de Requisitos de Ambiente em Sistemas Embarcados](http://wer.inf.puc-rio.br/WERpapers/artigos/artigos_WER10/martins.pdf)

#### Atividades Não Síncronas
* Pesquisar sobre Atualização OTA (Over-The-Air)
* [Atualização OTA na Wikipedia](https://pt.wikipedia.org/wiki/Over-the-air)
* [OTA para MicroPython](https://github.com/rdsmachado/ota_micropython)

---

### 10/08/2020
* Discussão do artigo: [GERSE: Guia de Elicitação de Requisitos para Sistemas Embarcados](http://www.inf.puc-rio.br/wer/WERpapers/artigos/artigos_WER12/paper_3.pdf)
* [Elicitação e Especificação de Requisitos para Sistemas Embarcados - Comparação TERASE & GERSE](https://www.cin.ufpe.br/~in1020/previous/2016.2/docs/works/inicial/Work_Reinaldo.pdf)
* Discussão sobre os projetos a serem desenvolvidos

#### Atividades Não Síncronas
* Edição da Tabela Gerse no GitHub individual
* [I2WAC: Uma Proposta para Gerenciamento de Irrigação Explorando Ciência de Situação na IoT](https://sol.sbc.org.br/index.php/semish/article/view/6571)
* [Códigos Exemplo em MicroPython](http://olaria.ucpel.edu.br/micropython/doku.php?id=codigos)

---

### 17/08/2020

#### Projetos Individuais - Etapa 1

* Entrega: código documentado com exemplos de operação.
* Apresentação: explicar a "arquitetura do software" caracterizando a troca de informações entre as partes do códigos.
* Discussão do andamento: 31/08/2020
* Finalização: 14/09/2020

**Kaller:** Configurar o acesso do embarcado a uma rede wi-fi, bem como a frequencia de piscagem de dois leds. Para confirmar que o embarcado está em rede deverá ser postada uma mensagem em um broker MQTT a cada 15 segundos.

**Lucas:** implementar uma rotina de OTA em MicroPython que será disparada sempre que o embarcado reiniciar. A medida que for ocorrendo deverá ser feito um log das operações realizadas empregando um Broker MQTT. Criar uma rotina para piscar dois leds como insumo de software a ser atualizado.

**Bruno:** criar um mecanismo simular ao Cron e sua Crontab em MicroPython apenas para minutos. Nos momentos agendados irá ser postada uma mensagem via MQTT e também um led será piscado. Vide sintaxe abaixo:
* mm 
* 10 será ativado aos 10 minutos de todas as horas
* 25 será ativado aos 25 minutos de todas as horas
* 33 será ativado aos 33 minutos de todas as horas

**Wellington:** implementar uma rotina que grave e leia informações em uma nuvem. Dependendo do que for lido serão ligados ou não dois leds de forma independente, ao iniciar e termnar a rotina, deverão ser gravadas strings na nuvem que caracterizem o início e o término da mesma.

**Gustavo**: conceber uma rotina de integração do embarcado com o Google Assistant. A partir de um comando de ligar e desligar uma rotina será ativada e/ou desativada.

---

### 24/08/2020
* [Diagramas de Sequencia Gerados a Partir de Texto](https://sourceforge.net/projects/sdedit/)
* [Editor on-line de Diagramas de Sequencia](https://online.visual-paradigm.com/pt/diagrams/solutions/free-sequence-diagram-editor-online/)

---

### 31/08/2020

* **Protolocos:**
    * A Organização Internacional de Normalização [ISO](https://pt.wikipedia.org/wiki/Organiza%C3%A7%C3%A3o_Internacional_de_Normaliza%C3%A7%C3%A3o) propôs o Modelo [OSI](https://pt.wikipedia.org/wiki/Modelo_OSI) 
    * [Apresentação Prof. Ronaldo Ramos](https://pt.slideshare.net/JanielesAraujo/protocolos-48853754)

**Primeira Atividade Avaliativa**

**Objetivo:** cada aluno irá estudar um dos protocolos atuais para Internet das Coisas, caracterizando as motivações e objetivos para sua criação, seus princípios operacionais, bem como as situações em que acontece o seu emprego na IoT. Na medida do possível comparar com os outros protocolos.

**Resultado:** deverá ser elaborada uma apresentação com duração de no máximo 10 minutos 

**Data apresentação:** 14/09/2020

* Bruno Lopes Soares	- COAP
* Gustavo Ribeiro Iribarrem	- REST & RESTfull
* Kaller Moraes Gonçalves	- LoRaWAN
* Lucas Kerstner Penning	- XMPP-IoT
* Wellington Weikamp Porto - SIGFOX

### 07/09/2020
* Feriado do Dia da Independência

### 14/09/2020
* Apresentação dos Protocolos Estudados pela Turma


### 21/09/2020
* [To Pull or Push IoT Data? That is the Question](https://www.sevone.com/news/blog/to-pull-or-push-iot-data-that-is-the-question/)
* Apresentação do Estado Atual dos Projetos pela Turma

### 28/09/2020

* Para o dia 19/10/2020 Definir os requisitos do Projeto a ser desenvolvido (no mínimo):
  * **Utilizar o Wiki do Repositório para as especificações.**
  * Nome (Name)
  * Objetivo (Purpose)
  * Entradas (Inputs)
  * Saídas (Outputs)
  * Funcionalidades (Functions)
  * Desempenho (Performance) - caso necessário
  * Potência (Power) - obrigatório se for operar a bateria

* Livro Associado:
  * Computer as Components: Principles of Embedded Computing System Design

* Slides:
  * [Metodologia de Desenvolvimento de Sistemas Embarcados](https://pt.slideshare.net/AlexandreAugustoGiron/metodologias-de-desenvolvimento-de-sistemas-embarcados)
  
### 05/10/2020

* Finalização da **Primeira Avaliação**

* Revisando os Projetos da Turma:
  * [30+ MicroPython Projects, Tutorials and Guides with ESP32/ESP8266](https://randomnerdtutorials.com/projects-esp32-esp8266-micropython/)
  
* Projetos:
  * **Bruno: MultiSensoriamento Explorando a Integração de Embarcados com uma Nuvem Computacional** 
    * Aplicação na Nuvem (PHP + HTML + CSS + MySQL) <--> [JSON + MQTT] <--> Embarcado (ESP32 + MicroPython)
        * Aplicação na Nuvem vai exibir valores sensoriados pelo Embarcado: último valor, lista de valores, gráfico
        * Aplicação na Nuvem vai configurar o Embarcado com frequência de leitura de cada um dos sensores envolvidos. Utilizar a sintaxe da Crontab para especificar o comportamento das leituras dos sensores
        * O embarcado vai fazer o sensoriamento e enviar o valor lido para a Aplicação na Nuvem.
        * O embarcado ao receber a configuração de leitura dos diferentes sensores da Aplicação em Nuvem irá gravar em um arquivo, persistindo a informação caso falte energia.
        * Empregar JSON como padrão para troca de dados entre a Aplicação na Nuvem e o Embarcado
        * Empregar MQTT para as comunicações
        * Empregar NTP (Network Time Protocol) no Embarcado

  * **Kaller: Sistema Inteligente de Irrigação**
    * Aplicação Console em Python <--> Embarcado
       * Aplicação Console especifica os horários para irrigação
       * Aplicação Console especifica o período para avaliação da irrigação (para avaliação serão utilizados sensores de umidade e temperatura)
       * A cada período de tempo especificado pela aplicação é avaliada pelo embarcado a necesidade de irrigação e o usuário é alertado
       * A Aplicação Console a qualquer momento pode comandar o início da irrigação
       * A Aplicação Console a qualquer momento pode comandar a finalização da irrigação
       * O embarcado pode considerar a previsão de chuva nas próximas horas
       * Empregar MQTT para as comunicações
       * Empregar NTP (Network Time Protocol) no Embarcado
 
  * **Lucas: Gerenciamento de Embarcados com Recurso de OTA**
    * Interface baseada em Bot Telegram <--> Embarcado
      * Verficação de aspectos operacionais: uptime, versão de software, sensores instalados, horário
      * Especificação de parâmetros de OTA: período de verificação de atualizações
      * Comandos de OTA: atualizar imediatamente, atualizar imediatamente na versão X.XX
      * Comandos gerais: reiniciar, executar determinado procedimento
      * Envio períodico de informações do Embarcado via Bot
      
  * **Gustavo:**
  
  * **Wellington: IoT Cloud**
    * API que irá permitir o embarcado criar e postar e deletar informações sensoriadas
      * Funcionalidade para permitir ao embarcado criar entrada para um determinado sensor
      * Funcionalidade para gravar as informações provenientes do embarcado
      * Funcionalidade para exibir as informações já gravadas
      * Aplicação Web para gerenciar o IoT Cloud
      * Aplicação no embarcado para criar sensores e popular com valores o IoT Cloud
      
### 12/10/2020  
   
* Feriado Nacional - Nossa Senhora Aparecida - Padroeira do Brasil
   
### 19/10/2020

* Primeiro Momento de Discussão dos Projetos da Turma


### 26/10/2020 ###

* Discussão dos Wikis dos Projetos de cada aluno.

### 02/11/2020 ###

* Feriado de Finados

### 09/11/2020 ###

* **Entrega do Relatório: 07/12/2020**

O Relatório pode ser feito no wiki do repositório do projeto ou em um editor de texto de preferência do projetista.

#### Composição do Relatório: ####
* Nome do Projeto

* Introdução:
    * Motivação
    * Objetivos (objetivo geral e objetivos específicos)
    
* Composição do Projeto
    * Figura com a arquitetura mostrando os "componentes" que formam o projeto
    * Breve descrição dos componentes de hardware e software que formam a arquitetura. 
      * Componentes de Hardware:
        * descrição do embarcado (com um link)
        * descrição do sensor 1 (com link)
        * descrição do sensor 2
        * descrição do desktop (hardware e sistema operacional)
        * ...
      * Compnentes de Software
        * descrição do protocolo MQTT (com link)
        * descrição da estrutura de armazenamento das variáves utilizadas (Banco de Dados)
        * Servidor Web (Apache)
        * HTML
        * CSS
        * GitHub
        * Componente 1 desenvolvidos para o Projeto (desenvolvido pelo aluno)
        * ...
        * Componente n desenvolvidos para o Projeto (desenvolvido pelo aluno)
    
  * Funcionalidades do Projeto
    * Nome da Funcionalidade 1 e sua descrição (Cada funcionalidade irá ter descritas as suas entradas e saídas, e como as mesmas são tratadas)
    * Funcionalidade 2
    * ...
    * Funcionalidade n
    * OBS. incluir um Fluxograma ou um Diagrama de Sequencia em UML, para cada funcionalidade ou grupo destas

### 16/11/2020 ###
* [Semana da Tecnologia em Saúde](http://olaria.ucpel.edu.br/sts2020)


### 23/11/2020 ###
* **Entendendo Microserviços:**
  * [Microservices.io](https://microservices.io/)
  * [Microserviços pela RedHat](https://www.redhat.com/pt-br/topics/microservices)
  * [Livros sobre Microserviços](https://blog.andrefaria.com/melhores-livros-sobre-microservices-microservicos)
* **Embarcados Experience 2020:**
  * [Informações sobre o Evento](https://www.embarcados.com.br/inscricao-embarcados-experience-2020/)

### 30/11/2020 ###

* **Segunda Avaliação da Disciplina**

## Links Relativos à Disciplina:

#### Plataformas de Software:
* [IFTTT](https://ifttt.com) - Contribuição de **Lucas Penning**
* [Robot Operating System](https://www.ros.org/)
* [Mosquitto](http://test.mosquitto.org/)

### Desenvolvendo Aplicações Móveis ###
* [Flutter do Google](https://flutter.dev/)
* [React Native](https://reactnative.dev/)

#### Eventos envolvendo Embarcados:
* [Brazilian Symposium on Computing Systems Engineering](https://sbesc.lisha.ufsc.br/)
* https://www.embarcados.com.br/sistemas-embarcados-e-microcontroladores/

#### Fabricação de Embarcados:
* [easyEDA](https://easyeda.com/)
* [PCBWay](https://www.pcbway.com)

#### Materiais sobre a Linguagem Python:
* [Guia de linguagem Python - DevMedia](https://www.devmedia.com.br/python/)
* [Lendo Ocupação de CPU e Memória em Python](https://www.it-swarm.dev/pt/python/como-obter-cpu-atual-e-ram-uso-em-python/958548632/)

#### Sistemas Embarcados em outras Instituições:
* [Disciplina "Sistemas Embarcados" na UFPEL](https://institucional.ufpel.edu.br/disciplinas/cod/1110070)

#### Protocolo MQTT
* Brokers:
  * [Brokers MQTT gratuitos e pagos para utilizar em projetos da IoT](https://diyprojects.io/8-online-mqtt-brokers-iot-connected-objects-cloud/#.XzfHmEl7nUI)
  * [IoTicos](https://ioticos.org/mqtt/login)
  * [DIoTY](http://www.dioty.co/)
* Dicas de Utilização:
  * [Material da Kasetsart University](https://www.cpe.ku.ac.th/~cpj/219335/slides/04-remote.pdf)
* MQTT no MicroPython:
  * [Robust UMQTT2](https://pypi.org/project/micropython-umqtt.robust2/)

#### Cron & MicroPython
* [Simple CRON for MicroPython](https://fizista.github.io/micropython-scron/html/index.html)

#### Criando Documentações
* [Sphinx](https://www.sphinx-doc.org/en/master/) - [Exemplo](http://docs.micropython.org/en/latest/) (Documentação Micropython)
* [Markdown](https://guides.github.com/features/mastering-markdown/) - Utilizado no GitHub

#### Ferramentas de Produtividade
* [Trello](https://trello.com/)
* [Notion](https://www.notion.so/)
* [Redmine](https://www.redmine.org)

#### Ferramentas para Construção de Fluxogramas
* [Draw.Io](http://draw.io)  - Contribuição de **Kaller Gonçalves**
* Google Docs

#### Ferramentas de Desenvolvimento
* [TotalCross - GUI Generator](https://totalcross.com)

### Diagramas de Apoio
* [Diagramas SE 2020](https://docs.google.com/presentation/d/1nzW87X-IIwwtUQdFPp_Pf1JqQ-x70nObhFrLf_DWIzs/)

### Exemplos de Projetos
* [Osciloscópio](http://olaria.ucpel.edu.br/scfu-2020/lib/exe/fetch.php?media=208277.pdf)
