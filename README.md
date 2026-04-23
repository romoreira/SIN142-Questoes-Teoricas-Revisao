# QUESTIONS

## SIN 142 - Sistemas Distribuídos

**Professor:** Rodrigo Moreira  
**Instituição:** UFV  


---

## Capítulo 1, Caracterização de Sistemas Distribuídos

1.  Cite cinco tipos de recursos de hardware e cinco tipos de recursos de dados ou software que podem ser compartilhados em um sistema distribuído. Dê exemplos práticos desse compartilhamento.
2.  Como os relógios de dois computadores ligados por uma rede local poderiam ser sincronizados sem recorrer a uma fonte externa de tempo? Quais fatores limitam a precisão desse procedimento? Como esse problema muda em escala de Internet?
3.  Em jogos online massivos, quais são as vantagens de uma abordagem baseada em servidor único para manter o estado global do jogo? Quais problemas essa abordagem traz e como poderiam ser mitigados?
4.  Compare computação em nuvem com o modelo cliente-servidor tradicional. O que há de realmente novo na noção de cloud computing?
5.  Um servidor implementado em C++ disponibiliza um objeto que será acessado por clientes em Java, executando em máquinas diferentes e heterogêneas. Quais problemas de heterogeneidade precisam ser resolvidos para permitir a invocação remota de métodos?
6.  Suponha que um objeto distribuído possua operações públicas e operações protegidas, acessíveis apenas por usuários autorizados. Quais problemas precisam ser resolvidos para garantir esse controle de acesso? E quais problemas adicionais surgem quando a operação protegida envolve dados sigilosos?
7.  Quando um cliente invoca um método em um objeto servidor, quais são os três principais componentes de software que podem falhar? Dê exemplos e discuta como o sistema pode tolerar essas falhas.
8.  Um servidor mantém um objeto compartilhado acessado por múltiplos clientes. Quais são os argumentos a favor e contra a execução concorrente das requisições? Dê um exemplo de interferência entre operações e explique como evitá-la.

---

## Capítulo 2, Modelos de Sistema

1.  Apresente três exemplos específicos e contrastantes dos níveis crescentes de heterogeneidade observados em sistemas distribuídos contemporâneos.
2.  Quais problemas decorrem do forte acoplamento entre entidades comunicantes em abordagens de invocação remota? Que vantagens podem surgir quando há desacoplamento no espaço e no tempo?
3.  Descreva a arquitetura cliente-servidor de uma grande aplicação da Internet, como Web, e-mail ou grupos de notícias.
4.  Em sistemas peer-to-peer, os hosts costumam ser computadores pessoais localizados em casas ou escritórios. Quais implicações isso traz para a disponibilidade e a segurança dos dados compartilhados? Até que ponto a replicação reduz essas fragilidades?
5.  Esboce uma solução em três camadas para o sistema distribuído de uma locadora de veículos. Discuta benefícios e desvantagens quanto a desempenho, escalabilidade, tolerância a falhas e manutenção.
6.  Explique, com um exemplo concreto, o dilema apresentado pelo argumento fim a fim no contexto do middleware para aplicações distribuídas confiáveis.
7.  Por que, em geral, não é possível estabelecer um limite rígido para o tempo de resposta de um servidor simples em um sistema distribuído? O que seria necessário para impor esse limite e por que isso costuma ser impraticável?
8.  Considere dois serviços de comunicação assíncronos com diferentes tipos de falha. Como classificar as falhas de cada serviço com relação às propriedades de validade e integridade? Em quais condições um serviço pode ser dito confiável?
9.  Descreva ocorrências possíveis dos principais tipos de ameaças de segurança na Internet, incluindo ameaças a processos, canais de comunicação e ataques de negação de serviço.

---

## Capítulo 3, Redes e Interconexão

1.  Um cliente envia uma requisição de 200 bytes e recebe uma resposta de 5000 bytes. Estime o tempo total da operação considerando comunicação sem conexão, com conexão e execução local na mesma máquina.
2.  A Internet é grande demais para que cada roteador mantenha rotas detalhadas para todos os destinos. Como o esquema de roteamento da Internet lida com essa limitação?
3.  Qual é a função de um switch Ethernet? Que tipo de tabela ele mantém e como essa tabela é utilizada?
4.  Como o argumento fim a fim influenciou o desenho da Internet? O que mudaria para a Web se o IP fosse substituído por um protocolo de rede orientado a circuito virtual?
5.  Compare UDP e TCP na implementação de aplicações como terminal remoto, transferência de arquivos, descoberta de usuários, navegação na Web e RPC.
6.  Como pacotes enviados por uma rede de longa distância podem chegar fora de ordem ao destino? Por que isso não ocorre da mesma forma em uma rede local?
7.  Quais são as desvantagens de usar broadcast no nível de rede para localizar recursos em uma Ethernet ou em uma intranet? Em que medida o multicast Ethernet melhora esse cenário?
8.  Proponha um esquema melhor que o Mobile IP para fornecer acesso a um servidor web em um dispositivo móvel que alterna entre rede celular e conexão cabeada em diferentes locais.
9.  Como você configuraria um firewall para proteger a rede local de uma instituição? Que tipos de tráfego de entrada e saída deveriam ser interceptados?
10.  Como um computador recém-conectado a uma Ethernet descobre os endereços IP dos servidores locais e como traduz esses endereços para endereços Ethernet?
11.  Firewalls podem impedir ataques de negação de serviço? Que outras estratégias podem ser usadas para enfrentar esse tipo de ataque?

---

## Capítulo 4, Comunicação entre Processos

1.  Em que situações pode ser útil que uma mesma porta tenha vários receptores?
2.  Um servidor cria uma porta para receber requisições de clientes. Quais são os principais problemas de projeto relacionados ao nome dessa porta e à forma como os clientes a descobrem?
3.  Compare o envio de dados por datagramas UDP com o envio por streams. Quais diferenças de comportamento e de uso ficam evidentes nessa comparação?
6.  Escreva, em pseudocódigo, um algoritmo de serialização que mostre como classes, instâncias e referências são tratadas durante o processo de serialização de objetos.
7.  Por que dados binários não podem ser representados diretamente em XML de forma natural? Quais são as vantagens e desvantagens de usar base64?
8.  Defina uma classe para representar referências remotas a objetos. Que informações ela deve armazenar e como cada método de acesso seria usado por protocolos de mais alto nível?
9.  Projete um esquema que use retransmissões para reduzir perdas em multicast IP, considerando múltiplos emissores e baixa taxa média de perda.
10.  Em que sentido uma solução baseada em retransmissão para multicast IP ainda difere da definição formal de multicast confiável?
11.  Construa um cenário em que multicasts enviados por clientes diferentes sejam entregues em ordens distintas para membros do grupo. Como os destinatários poderiam corrigir esse problema?
12.  Qual é o impacto das redes overlay sobre a arquitetura da Internet e sobre a forma como o programador passa a enxergar a rede?
13.  Quais são os principais argumentos a favor da adoção de supernós em sistemas como o Skype?
14.  Em MPI, a operação `MPI_Rsend` assume que o receptor já está pronto para receber. Que otimizações essa suposição permite e o que pode acontecer se ela for falsa?

---

## Capítulo 5, Invocação Remota

1.  Como projetar uma versão de `doOperation` que use timeout e retransmissão de requisições? Que decisões precisam ser tomadas para informar corretamente o chamador quando não houver resposta?
2.  Descreva um cenário em que um cliente possa receber a resposta de uma chamada remota anterior em vez da resposta da chamada atual.
3.  De que forma o protocolo requisição-resposta mascara a heterogeneidade de sistemas operacionais e redes de computadores?
4.  Discuta se as seguintes operações são idempotentes, pressionar o botão do elevador, sobrescrever um arquivo, anexar dados a um arquivo. Uma operação precisa ser sem estado para ser idempotente?
5.  Quais escolhas de projeto ajudam a minimizar a quantidade de dados de resposta que o servidor precisa manter? Compare os requisitos de armazenamento dos protocolos RR e RRA.
6.  Por quanto tempo um servidor deveria manter respostas não confirmadas no protocolo RRA? Ele deveria reenviar respostas periodicamente?
7.  Por que o número de mensagens trocadas pode ser mais importante para o desempenho do que o volume total de dados transmitidos? Como funcionaria uma variante do RRA com confirmação piggyback?
8.  Em um serviço de eleição com métodos `vote` e `result`, identifique quais parâmetros são de entrada e quais são de saída.
9.  Quais semânticas de invocação podem ser obtidas quando o protocolo requisição-resposta é implementado sobre TCP, considerando que conexões podem ser interrompidas em diferentes momentos?
10.  Em um serviço de votação, seria aceitável usar semântica de chamada *at-least-once* ou seria mais adequado adotar *at-most-once*? Justifique.
11.  Ao implementar um protocolo requisição-resposta sobre um serviço com falhas por omissão, como a suposição de um tempo máximo de execução e comunicação simplifica a implementação?
12.  Esboce uma implementação do serviço de eleição que preserve consistência mesmo quando múltiplos clientes votam concorrentemente.
13.  Como garantir, em uma implementação RMI do serviço de eleição, que todos os votos sejam preservados mesmo se o processo servidor falhar?
14.  Como mudaria o projeto de `doOperation` se argumentos e resultados fossem transmitidos como objetos por meio de `ObjectOutputStream` e `ObjectInputStream` sobre TCP?
15.  Calcule o tempo para duas requisições remotas em um cliente monothread e em um cliente com duas threads concorrentes. Há necessidade de invocação assíncrona se cliente e servidor já forem multithread?
16.  Projete uma tabela de objetos remotos que suporte tanto tradução entre referências locais e remotas quanto coleta de lixo distribuída.
17.  Em uma versão simplificada de coleta de lixo distribuída baseada apenas em `addRef` e `removeRef`, quais efeitos poderiam ser causados por falhas de processo e comunicação? Como contorná-los sem usar leases?

---

## Capítulo 6, Comunicação Indireta

1.  Por que a comunicação indireta pode ser particularmente adequada em ambientes voláteis? Esse benefício decorre do desacoplamento no tempo, no espaço, ou de ambos?
2.  Se mensagens forem endereçadas a nomes e esses nomes forem resolvidos por DNS, isso produz o mesmo nível de indireção de um sistema realmente desacoplado?
3.  É possível construir um paradigma de comunicação que seja acoplado no espaço e desacoplado no tempo? O e-mail se encaixa nessa categoria?
4.  No modelo de *queued RPC*, chamadas remotas ficam enfileiradas até que o destinatário esteja disponível. Em que sentido isso caracteriza desacoplamento temporal?
5.  Se um paradigma de comunicação é assíncrono, isso significa necessariamente que ele é desacoplado no tempo? Explique com exemplos.
6.  Em comunicação de grupo, dê exemplos que ilustrem a diferença entre ordenação causal e ordenação total.
7.  Imagine uma aplicação de alarmes com vários tipos de evento, como incêndio, inundação e intrusão. Quais requisitos de confiabilidade e ordenação essa aplicação teria?
8.  Proponha o projeto de um serviço de caixa postal de notificações para múltiplos assinantes, permitindo que cada assinante controle quando deseja receber as notificações.
9.  Por que abordagens de publicação e assinatura baseadas em canais podem ser implementadas facilmente com comunicação de grupo? Por que essa estratégia é menos adequada para filtros baseados em conteúdo?
10.  Como o baixo acoplamento das filas de mensagens ajuda na integração de aplicações corporativas? Relacione isso ao desacoplamento no tempo e no espaço.
11.  Em que aspectos a memória compartilhada distribuída é adequada ou inadequada para sistemas cliente-servidor?
12.  Para aplicações tolerantes a falhas, o que tende a ser preferível, passagem de mensagens ou memória compartilhada distribuída? Justifique.
13.  Se um sistema DSM for implementado em middleware, de forma neutra em relação à plataforma e sem apoio de hardware, como lidar com representações distintas de dados em máquinas heterogêneas? Essa solução se estende a ponteiros?
14.  Como implementar o equivalente a uma chamada de procedimento remoto usando um espaço de tuplas? Quais seriam as vantagens e as desvantagens?
15.  Como implementar um semáforo usando espaço de tuplas?

---

## Capítulo 10, Sistemas Peer-to-Peer

1.  Aplicações como o Napster sofriam limitações de escalabilidade devido ao índice centralizado. Que outras soluções para indexação de recursos podem ser adotadas?
2.  Compare a adequação das estratégias de indexação para três cenários, compartilhamento de mídia, armazenamento de longo prazo de conteúdo arquivado e armazenamento distribuído de arquivos de leitura e escrita.
3.  Quais são as principais garantias que usuários esperam de servidores convencionais, como servidores web e servidores de arquivos?
4.  As garantias de servidores convencionais podem ser violadas por danos físicos, erros administrativos, ataques bem-sucedidos e falhas de hardware ou software. Dê exemplos de incidentes para cada caso e discuta quando eles configuram quebra de confiança ou ato criminoso.
5.  Em sistemas peer-to-peer, confiança e volatilidade dos nós dependem de fatores humanos e operacionais. Como atributos como propriedade, localização geográfica, conectividade e jurisdição afetam políticas de posicionamento de dados?
6.  Avalie a disponibilidade e a confiabilidade de computadores pessoais do seu ambiente em termos de tempo ativo, consistência de software e segurança. Com base nisso, discuta a viabilidade de um serviço de compartilhamento de dados.
7.  Por que o uso de um hash seguro para identificar objetos e rotear mensagens até eles pode ser considerado resistente a adulteração? Que propriedades o hash precisa ter?
8.  Sistemas peer-to-peer realmente conseguem oferecer anonimato para clientes e para hosts que oferecem recursos? Como a resistência a ataques contra o anonimato poderia ser aumentada?
9.  Em sistemas como Kademlia, a distância entre GUIDs é baseada em XOR. Como isso ajuda na manutenção das tabelas de roteamento? O XOR satisfaz propriedades adequadas para uma métrica de distância?
10.  Compare as estratégias de busca *expanded ring search* e *random walk* em sistemas peer-to-peer não estruturados, destacando em que situações cada uma tende a ser mais eficaz.

---

## Capítulo 11, Segurança

1.  Descreva políticas de segurança física de uma organização e mostre como elas poderiam ser traduzidas para regras de um sistema computadorizado de controle de acesso por portas.
2.  De que formas o e-mail convencional é vulnerável a espionagem, falsificação de identidade, adulteração, repetição de mensagens e negação de serviço? Como cada ameaça poderia ser mitigada?
3.  As trocas iniciais de chaves públicas são vulneráveis a ataques man-in-the-middle. Quais defesas podem ser usadas contra esse tipo de ataque?
4.  Quais passos dois usuários que utilizam PGP devem seguir antes de trocar mensagens com garantias de privacidade e autenticidade? O quanto da negociação inicial poderia ser invisível para o usuário?
5.  Como enviar uma mensagem segura a uma grande lista de destinatários usando PGP ou esquema semelhante? Que alternativa seria mais simples e rápida quando a lista é usada frequentemente?
6.  A implementação do algoritmo TEA apresentada no capítulo não é portável entre todas as arquiteturas. Por quê? Como uma mensagem criptografada poderia ser transmitida de modo a ser corretamente decriptada em outras arquiteturas?
7.  Estime o tempo necessário para quebrar por força bruta uma chave DES de 56 bits em um computador de 2000 MIPS. Repita a análise para uma chave IDEA de 128 bits e extrapole para um processador paralelo de 200000 MIPS.
8.  No protocolo de autenticação de Needham e Schroeder com chaves secretas, por que a versão simplificada da mensagem 5 não é segura?

---


