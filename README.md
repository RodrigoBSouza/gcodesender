# Mini CNC de Baixo Custo - Documentação do Projeto

## Descrição do Projeto

Este repositório contém a documentação e o código-fonte para a construção de uma Mini CNC de baixo custo. A máquina utiliza drives de DVD reutilizados, integrados de maneira criativa com uma plataforma de suporte em madeira, e é controlada por um Arduino UNO R3. A mini CNC é projetada para realizar desenhos de baixa resolução coordenando uma caneta nos eixos X, Y e Z.

## Conteúdo do Repositório

1. **Descrição do Funcionamento e Uso:**
   ## Descrição de Funcionamento

### Montagem da Base de Madeira

Inicialmente, uma base de madeira foi construída para facilitar os testes preliminares, proporcionando uma visão antecipada do potencial desfecho do projeto. A estrutura finalizada apresenta uma estética agradável e respeita os parâmetros estabelecidos, consolidando a escolha da base de madeira como suporte definitivo.

### Alinhamento dos Drives

O primeiro desafio foi alinhar os drives de DVD sobre a estrutura de madeira e posicionar o drive de disquete em relação ao drive de DVD. Esse processo exigiu uma busca meticulosa pela precisão, evitando qualquer tensão nos motores e eixos durante a geração dos desenhos essenciais para os testes subsequentes.

### Conexões Externas e Protoboard

Após garantir o alinhamento preciso, foram feitas as conexões externas utilizando uma protoboard como interface para a ligação dos motores. Isso assegurou a integridade e funcionalidade do sistema. A Figura abaixo ilustra o protótipo montado sobre a base de madeira, destacando o cuidadoso processo de montagem.

![Imagem do WhatsApp de 2023-11-11 à(s) 20 28 37_255ecdee](https://github.com/RodrigoBSouza/gcodesender/assets/87902323/91301d49-d83e-47e9-8b9f-d4b2d8a9438a)

### Configuração do Software

A primeira fase da configuração no software envolve o envio da biblioteca "grbl.h" para a placa Arduino UNO R3. O GRBL, uma ferramenta de código aberto, destaca-se pelo desempenho exemplar na gestão do movimento de máquinas móveis.

### Uso do Inkscape para Conversão de Desenhos

O software utilizado para converter desenhos ou imagens em formato vetorial é o Inkscape, uma aplicação de qualidade profissional de código aberto. Dedicado à manipulação de gráficos vetoriais, o Inkscape opera conforme o padrão aberto SVG (Scalable Vector Graphics). Através dele, a imagem é moldada conforme as necessidades específicas e os parâmetros da mini CNC.

### Universal Gcode Sender

O Inkscape desempenha um papel crucial na geração da imagem completa, incluindo parâmetros e configurações relevantes. Essa imagem é carregada no Universal Gcode Sender, um software em Java que atua como interface com controladores CNC avançados, como GRBL e TinyG. O Universal Gcode Sender estabelece a comunicação com o conjunto de placas, permitindo a execução do desenho na mini CNC. A configuração desse processo pode ser visualizada na figura abaixo.

![Texto Alternativo](https://raw.githubusercontent.com/RodrigoBSouza/gcodesender/main/assets/87902323/8bf815d9-e379-41f4-bf0b-9ee73c39997c)

2. **Software Desenvolvido e Documentação de Código:**
   - O código-fonte está disponível no diretório: https://github.com/RodrigoBSouza/gcodesender/tree/main

3. **Descrição do Hardware Utilizado:**
   - Plataformas de desenvolvimento: Arduino UNO R3
   - Sensores: Drives de DVD e Drive de Disquete
   - Atuadores: Motores de passo
   - Outros: CNC Shield A4988, Drivers de Potência

## Resumo do Artigo

A montagem da Mini CNC revelou-se um sucesso, proporcionando uma visão prática e funcional do projeto proposto. A base de madeira, cuidadosamente confeccionada, demonstrou ser uma escolha sólida para suportar os componentes da máquina. O alinhamento preciso dos drives de DVD e do drive de disquete, apesar dos desafios iniciais, foi alcançado, garantindo a estabilidade durante as operações. As conexões externas, realizadas através de uma protoboard, contribuíram para a integridade e funcionalidade do sistema, permitindo uma fácil manutenção e ajustes. O protótipo montado sobre a base de madeira, evidenciado na Figura 6, destaca a meticulosidade do processo de montagem, resultando em uma estética agradável e compacta.

A configuração do software, envolvendo o uso da biblioteca "grbl.h" e as ferramentas como Inkscape e Universal Gcode Sender, revelou-se eficiente e acessível. A comunicação entre o Arduino e os drives de potência foi bem-sucedida, proporcionando um controle preciso dos motores e, consequentemente, dos movimentos da caneta.

Os testes de funcionamento, incluindo a execução de desenhos simples, confirmaram a capacidade da Mini CNC em realizar suas tarefas previstas. A resolução, embora limitada, mostrou-se suficiente para experimentações artísticas e prototipagem básica. Os resultados obtidos destacam a viabilidade e acessibilidade desse projeto, representando um passo significativo em direção à democratização da tecnologia CNC.

Em suma, a montagem bem-sucedida da Mini CNC não apenas valida a abordagem proposta, mas também oferece uma plataforma pronta para experimentação, aprendizado prático e aplicações criativas, promovendo a acessibilidade e sustentabilidade no contexto da fabricação digital.

## Considerações Finais

Este repositório é uma fonte abrangente para quem busca construir e entender a Mini CNC de baixo custo.
