# Questionário CE — Semanas 1 a 7

Formato: 10 questões por semana, sendo 3 fáceis, 4 médias e 3 difíceis. Cada questão possui 5 alternativas (A–E), gabarito, explicação detalhada e um prompt individual para infográfico no ChatGPT.

**Revisão:** cada questão agora traz a(s) fonte(s) PDF usada(s) como base, indicada(s) pelo caminho dentro de `/dados/CE/`.

\---

## Semana 1 — Introdução à Programação Paralela e Sistemas Distribuídos

### S1Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Computação paralela pode ser definida como:

  * **A.** Execução de um programa em uma única CPU, sempre uma instrução por vez.
  * **B.** Uso simultâneo de múltiplos recursos computacionais para resolver um problema.
  * **C.** Execução de programas sem qualquer comunicação entre tarefas.
  * **D.** Técnica exclusiva de supercomputadores comerciais.
  * **E.** Substituição completa da programação sequencial por redes neurais.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 1/s1\_videoaula1.pdf; Semana 1/s1\_texto\_base-introducao\_a\_programacao\_paralela\_e\_distribuida.pdf
* **Explicação detalhada:** Computação paralela consiste em dividir um problema em partes que possam ser executadas ao mesmo tempo por múltiplos recursos, como vários núcleos, processadores ou computadores conectados em rede. O objetivo principal é reduzir o tempo de execução ou aumentar a capacidade de processamento.
* **Prompt para infográfico:** Crie um infográfico explicando computação paralela: definição, divisão do problema em partes, exemplos de recursos paralelos e comparação visual entre execução sequencial e paralela.

### S1Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** A fórmula básica de speedup é:

  * **A.** Tempo paralelo / tempo serial.
  * **B.** Número de threads / tempo de comunicação.
  * **C.** Tempo serial / tempo paralelo.
  * **D.** Tempo de sincronização / tempo total.
  * **E.** Eficiência / número de processadores.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 1/s1\_videoaula2.pdf
* **Explicação detalhada:** Speedup mede o quanto uma execução paralela é mais rápida em relação à execução serial. Se um programa leva 100 segundos serialmente e 25 segundos paralelamente, o speedup é 100/25 = 4.
* **Prompt para infográfico:** Crie um infográfico sobre speedup com fórmula, exemplo numérico e interpretação prática do resultado.

### S1Q3

* **Nível:** Fácil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** Avalie: I) Sistemas distribuídos usam computadores interligados por rede. II) Componentes coordenam ações por mensagens. III) Todo sistema distribuído possui relógio global perfeito.

  * **A.** V, V, V
  * **B.** F, V, F
  * **C.** V, F, V
  * **D.** V, V, F
  * **E.** F, F, V
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 1/Aprof 1 - Livro Sistemas Distribuidos Conceitos e Projetos Colourius - cap 1.pdf
* **Explicação detalhada:** Sistemas distribuídos têm componentes em computadores conectados em rede que se comunicam por troca de mensagens. Uma característica importante é justamente a ausência de um relógio global perfeitamente sincronizado.
* **Prompt para infográfico:** Crie um infográfico sobre sistemas distribuídos destacando rede, passagem de mensagens, ausência de relógio global e falhas independentes.

### S1Q4

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** A principal diferença entre concorrência e paralelismo é:

  * **A.** Concorrência sempre exige múltiplos processadores; paralelismo nunca exige.
  * **B.** Concorrência lida com múltiplas atividades em progresso; paralelismo executa atividades simultaneamente para desempenho.
  * **C.** Concorrência só existe em sistemas distribuídos.
  * **D.** Paralelismo é apenas alternância de tarefas em uma CPU.
  * **E.** Não há diferença conceitual entre os termos.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 1/s1\_texto\_base-introducao\_a\_programacao\_paralela\_e\_distribuida.pdf
* **Explicação detalhada:** Concorrência trata da estruturação de um programa com múltiplas atividades que podem progredir de forma intercalada. Paralelismo envolve execução simultânea real, normalmente para reduzir tempo de processamento.
* **Prompt para infográfico:** Crie um infográfico comparando concorrência e paralelismo com exemplos, objetivos e riscos.

### S1Q5

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Granularidade em programação paralela refere-se:

  * **A.** Ao tamanho do trabalho atribuído a cada tarefa antes de sincronizar/comunicar.
  * **B.** Ao número total de computadores da Internet.
  * **C.** À velocidade do clock da CPU.
  * **D.** Ao tipo de linguagem usada.
  * **E.** Ao tamanho físico do processador.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 1/s1\_videoaula2.pdf
* **Explicação detalhada:** Granularidade indica quão grandes ou pequenas são as partes em que o problema foi dividido. Granularidade fina gera muitas tarefas pequenas e mais comunicação; granularidade grossa gera tarefas maiores e menos sincronização.
* **Prompt para infográfico:** Crie um infográfico sobre granularidade fina versus grossa, mostrando relação entre computação, comunicação e sincronização.

### S1Q6

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) Decomposição; 2) Race condition; 3) Deadlock; 4) Balanceamento de carga. a) Dividir problema; b) Resultado depende da ordem; c) Tarefas bloqueadas; d) Distribuir trabalho adequadamente.

  * **A.** 1-a, 2-c, 3-b, 4-d
  * **B.** 1-b, 2-a, 3-d, 4-c
  * **C.** 1-d, 2-c, 3-b, 4-a
  * **D.** 1-a, 2-b, 3-c, 4-d
  * **E.** 1-c, 2-d, 3-a, 4-b
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 1/s1\_texto\_base-introducao\_a\_programacao\_paralela\_e\_distribuida.pdf
* **Explicação detalhada:** Decomposição divide o problema em partes; race condition ocorre quando o resultado depende da ordem de execução; deadlock impede progresso por bloqueios mútuos; balanceamento de carga distribui trabalho entre recursos.
* **Prompt para infográfico:** Crie um infográfico com quatro desafios da programação paralela: decomposição, race condition, deadlock e balanceamento de carga.

### S1Q7

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Entre os desafios dos sistemas distribuídos, a escalabilidade significa:

  * **A.** Usar sempre o menor número possível de computadores.
  * **B.** Manter funcionamento adequado quando usuários, carga ou recursos aumentam.
  * **C.** Impedir a entrada de novos componentes no sistema.
  * **D.** Eliminar totalmente falhas de rede.
  * **E.** Centralizar todas as decisões em um único relógio global.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 1/Aprof 1 - Livro Sistemas Distribuidos Conceitos e Projetos Colourius - cap 1.pdf
* **Explicação detalhada:** Escalabilidade é a capacidade de o sistema continuar operando bem quando cresce em número de usuários, quantidade de dados, volume de requisições ou número de componentes.
* **Prompt para infográfico:** Crie um infográfico sobre escalabilidade em sistemas distribuídos com exemplos de crescimento de usuários, carga e recursos.

### S1Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Por que a ausência de relógio global é um problema importante em sistemas distribuídos?

  * **A.** Porque impede completamente qualquer comunicação.
  * **B.** Porque obriga todos os computadores a ficarem desligados.
  * **C.** Porque dificulta ordenar eventos e coordenar ações com precisão entre máquinas.
  * **D.** Porque torna desnecessária a passagem de mensagens.
  * **E.** Porque elimina problemas de concorrência.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 1/Aprof 1 - Livro Sistemas Distribuidos Conceitos e Projetos Colourius - cap 1.pdf
* **Explicação detalhada:** Em sistemas distribuídos, cada máquina possui seu próprio relógio, e sincronizá-los perfeitamente é inviável. Isso dificulta saber a ordem exata dos eventos, coordenar operações e detectar atrasos ou falhas.
* **Prompt para infográfico:** Crie um infográfico mostrando por que não há relógio global perfeito em sistemas distribuídos e como isso afeta ordenação de eventos e coordenação.

### S1Q9

* **Nível:** Difícil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Falhas independentes significam que um nó pode falhar sem todos falharem. II) Transparência busca ocultar complexidades do sistema. III) Heterogeneidade significa que todos os componentes são idênticos.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, F
  * **D.** F, V, V
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 1/Aprof 1 - Livro Sistemas Distribuidos Conceitos e Projetos Colourius - cap 1.pdf
* **Explicação detalhada:** Falhas independentes são típicas de sistemas distribuídos. Transparência procura esconder detalhes como localização, migração ou replicação. Heterogeneidade significa diversidade de hardware, software, redes e linguagens, não identidade.
* **Prompt para infográfico:** Crie um infográfico sobre desafios de sistemas distribuídos: falhas independentes, transparência e heterogeneidade.

### S1Q10

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** A eficiência paralela é importante porque:

  * **A.** Mostra se o speedup obtido é proporcional ao número de recursos usados.
  * **B.** Mede apenas o consumo de memória RAM.
  * **C.** É sempre igual a 100% em programas paralelos.
  * **D.** Ignora comunicação e sincronização.
  * **E.** Só se aplica a sistemas sem threads.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 1/s1\_videoaula2.pdf
* **Explicação detalhada:** A eficiência relaciona o speedup ao número de processadores/cores utilizados. Ela indica se os recursos adicionais estão sendo bem aproveitados ou se comunicação, sincronização e desequilíbrio estão reduzindo o ganho.
* **Prompt para infográfico:** Crie um infográfico explicando eficiência paralela, com fórmula, exemplo e fatores que reduzem eficiência.

\---

## Semana 2 — Programação Concorrente, Multicore, Threads e Flynn

### S2Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Um processador multicore é:

  * **A.** Um cluster de computadores independentes.
  * **B.** Um chip físico com mais de um núcleo de processamento.
  * **C.** Um sistema operacional distribuído.
  * **D.** Uma rede de sensores sem CPU.
  * **E.** Uma técnica exclusiva de armazenamento.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 2/s2-Texto Base 1 - Multicore – Definirtec.pdf
* **Explicação detalhada:** Multicore significa que um único processador físico contém vários núcleos capazes de executar tarefas simultaneamente, aumentando a capacidade de processamento.
* **Prompt para infográfico:** Crie um infográfico explicando multicore com desenho de um chip contendo vários núcleos e seus benefícios.

### S2Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Threads são úteis principalmente porque:

  * **A.** Permitem organizar múltiplas atividades dentro de um processo.
  * **B.** Eliminam a necessidade de sistema operacional.
  * **C.** Impedem qualquer bloqueio de E/S.
  * **D.** Nunca compartilham memória.
  * **E.** Só funcionam em clusters.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 2/S2-Sistemas Op Mod- 3ª Ed- 325-331.pdf; Semana 2/s2-SO Modernos 4 ed- 67-73.pdf
* **Explicação detalhada:** Threads permitem que uma aplicação tenha múltiplos fluxos de execução, como interface, cálculo e entrada/saída, muitas vezes compartilhando o mesmo espaço de endereçamento.
* **Prompt para infográfico:** Crie um infográfico mostrando um processo com várias threads e exemplos práticos de uso.

### S2Q3

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Na classificação de Flynn, SISD significa:

  * **A.** Múltiplas instruções, múltiplos dados.
  * **B.** Uma instrução, múltiplos dados.
  * **C.** Múltiplas instruções, um dado.
  * **D.** Uma instrução, um dado.
  * **E.** Sem instruções e sem dados.
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 2/s2\_revisitando\_aula\_01\_introducao\_programacao\_concorrente.pdf
* **Explicação detalhada:** SISD representa a arquitetura sequencial clássica: um fluxo de instruções operando sobre um fluxo de dados.
* **Prompt para infográfico:** Crie um infográfico da classificação de Flynn destacando SISD como modelo sequencial tradicional.

### S2Q4

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) SISD; 2) SIMD; 3) MISD; 4) MIMD. a) Uma instrução/um dado; b) Uma instrução/múltiplos dados; c) Múltiplas instruções/um dado; d) Múltiplas instruções/múltiplos dados.

  * **A.** 1-c, 2-d, 3-a, 4-b
  * **B.** 1-b, 2-a, 3-d, 4-c
  * **C.** 1-d, 2-c, 3-b, 4-a
  * **D.** 1-a, 2-c, 3-b, 4-d
  * **E.** 1-a, 2-b, 3-c, 4-d
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 2/s2\_revisitando\_aula\_01\_introducao\_programacao\_concorrente.pdf; Semana 2/s2\_videoaula3.pdf
* **Explicação detalhada:** Flynn classifica arquiteturas pelo número de fluxos de instruções e dados. SIMD é comum em vetorização; MIMD é comum em multiprocessadores e clusters.
* **Prompt para infográfico:** Crie uma matriz 2x2 da classificação de Flynn com significado e exemplo de cada categoria.

### S2Q5

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Em memória compartilhada UMA:

  * **A.** Todos os processadores acessam a memória com tempo uniforme.
  * **B.** Cada processador só acessa memória local.
  * **C.** Não existe espaço de endereçamento comum.
  * **D.** A comunicação ocorre apenas por mensagens de rede.
  * **E.** Não há caches.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 2/s2-SO Modernos 4 ed 364-366.pdf
* **Explicação detalhada:** UMA significa Uniform Memory Access. Os processadores compartilham um espaço de memória e o tempo de acesso é uniforme, exigindo mecanismos de coerência de cache.
* **Prompt para infográfico:** Crie um infográfico comparando UMA e NUMA, destacando acesso uniforme e coerência de cache.

### S2Q6

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Multithreading de granularidade fina alterna threads:

  * **A.** Apenas quando o computador reinicia.
  * **B.** Com alta frequência, até entre instruções.
  * **C.** Somente quando há falha permanente.
  * **D.** Nunca alterna threads.
  * **E.** Somente em sistemas sem cache.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 2/s2-Texto Base 2 - paralelismo\_no\_nivel\_de\_threads.pdf
* **Explicação detalhada:** Na granularidade fina, a troca entre threads é frequente para tentar esconder latências. Na granularidade grossa, a troca ocorre em eventos mais caros, como falhas de cache.
* **Prompt para infográfico:** Crie uma linha do tempo comparando multithreading de granularidade fina e grossa.

### S2Q7

* **Nível:** Média
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Threads de um mesmo processo podem compartilhar memória. II) Processos normalmente têm espaços de endereçamento separados. III) Compartilhamento elimina todos os problemas de sincronização.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, V
  * **D.** F, V, F
  * **E.** F, F, V
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 2/S2-Sistemas Op Mod- 3ª Ed- 325-331.pdf; Semana 2/s2-SO Modernos 4 ed- 67-73.pdf
* **Explicação detalhada:** Threads podem compartilhar dados, o que facilita comunicação interna, mas também cria riscos de corrida e exige sincronização. Processos são mais isolados por padrão.
* **Prompt para infográfico:** Crie um infográfico comparando processos e threads, destacando isolamento, compartilhamento e sincronização.

### S2Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** A coerência de cache é necessária em multiprocessadores porque:

  * **A.** Caches diferentes podem conter cópias do mesmo dado compartilhado.
  * **B.** Ela substitui a memória principal.
  * **C.** Ela elimina a necessidade de barramento.
  * **D.** Ela impede execução paralela.
  * **E.** Ela transforma MIMD em SISD.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 2/s2\_revisitando\_aula\_01\_introducao\_programacao\_concorrente.pdf; Semana 2/s2\_videoaula4.pdf
* **Explicação detalhada:** Quando múltiplos processadores possuem caches, um mesmo dado pode estar copiado em vários lugares. Se um processador altera o dado, os outros precisam ver uma versão coerente, por atualização ou invalidação.
* **Prompt para infográfico:** Crie um infográfico sobre coerência de cache com exemplo de dois núcleos acessando a mesma variável.

### S2Q9

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** SIMD é especialmente adequado para:

  * **A.** Substituir completamente sistemas operacionais.
  * **B.** Executar um único programa sem dados.
  * **C.** Sistemas onde cada processador executa instruções completamente diferentes sem relação.
  * **D.** Eliminar paralelismo de dados.
  * **E.** Aplicar a mesma operação sobre muitos dados, como vetores ou matrizes.
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 2/s2\_revisitando\_aula\_01\_introducao\_programacao\_concorrente.pdf; Semana 2/s2\_videoaula4.pdf
* **Explicação detalhada:** SIMD executa uma mesma instrução sobre múltiplos dados, sendo útil em processamento vetorial, imagens, matrizes e GPUs.
* **Prompt para infográfico:** Crie um infográfico mostrando SIMD aplicado a vetores: mesma operação sendo executada sobre vários elementos.

### S2Q10

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** O maior risco de usar threads com memória compartilhada sem controle é:

  * **A.** Conversão automática para computação em nuvem.
  * **B.** Impossibilidade de usar processadores multicore.
  * **C.** Ausência de qualquer paralelismo.
  * **D.** Redução obrigatória do número de instruções.
  * **E.** Condições de corrida e inconsistência de dados.
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 2/S2-Sistemas Op Mod- 3ª Ed- 325-331.pdf; Semana 2/s2-SO Modernos 4 ed- 67-73.pdf
* **Explicação detalhada:** Quando threads acessam e alteram os mesmos dados simultaneamente sem sincronização, a ordem das operações pode produzir resultados incorretos ou imprevisíveis.
* **Prompt para infográfico:** Crie um infográfico sobre race condition em threads, com exemplo simples de incremento concorrente de variável.

\---

## Semana 3 — Clusters, Grades Computacionais e Computação em Nuvem

### S3Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Um cluster computacional é:

  * **A.** Um grupo de computadores interligados que trabalham como recurso computacional conjunto.
  * **B.** Um único processador com vários registradores.
  * **C.** Uma linguagem de programação paralela.
  * **D.** Um tipo de arquivo compactado.
  * **E.** Um protocolo exclusivo de e-mail.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_cluster\_computacao\_de\_alto\_desempenho.pdf; Semana 3/s3\_texto\_base\_aspectos\_tecnicos\_envolvidos\_na\_construcao\_de\_um\_cluster.pdf
* **Explicação detalhada:** Clusters conectam computadores, geralmente por rede local, para executar tarefas de alto desempenho, alta disponibilidade ou balanceamento de carga.
* **Prompt para infográfico:** Crie um infográfico mostrando um cluster com nó mestre, nós de processamento e rede de interconexão.

### S3Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Um cluster Beowulf ficou conhecido por:

  * **A.** Proibir programação paralela.
  * **B.** Usar apenas supercomputadores proprietários caríssimos.
  * **C.** Usar PCs comuns, Linux e rede para obter alto desempenho com baixo custo.
  * **D.** Ser uma tecnologia exclusiva de celulares.
  * **E.** Eliminar a necessidade de hardware.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_aspectos\_tecnicos\_envolvidos\_na\_construcao\_de\_um\_cluster.pdf
* **Explicação detalhada:** O cluster Beowulf popularizou a ideia de construir alto desempenho usando componentes de mercado, software livre e bibliotecas de passagem de mensagens.
* **Prompt para infográfico:** Crie um infográfico sobre cluster Beowulf: origem, componentes comuns, Linux, rede e baixo custo.

### S3Q3

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Computação em nuvem caracteriza-se principalmente por:

  * **A.** Proibição de escalabilidade.
  * **B.** Uso obrigatório de um único computador local.
  * **C.** Ausência total de virtualização.
  * **D.** Oferta de recursos computacionais sob demanda pela rede.
  * **E.** Execução sem servidores físicos.
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_computacao\_em\_nuvem.pdf
* **Explicação detalhada:** A nuvem fornece recursos como processamento, armazenamento, bancos de dados e plataformas via rede, com elasticidade, provisionamento sob demanda e pagamento conforme uso.
* **Prompt para infográfico:** Crie um infográfico com os conceitos de nuvem: sob demanda, elasticidade, rede, pagamento por uso e serviços.

### S3Q4

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) Cluster; 2) Grid; 3) Nuvem; 4) Beowulf. a) Recursos heterogêneos e distribuídos entre organizações; b) PCs comuns em rede para HPC; c) Recursos sob demanda; d) Máquinas próximas cooperando como sistema.

  * **A.** 1-d, 2-a, 3-c, 4-b
  * **B.** 1-a, 2-d, 3-b, 4-c
  * **C.** 1-c, 2-b, 3-a, 4-d
  * **D.** 1-b, 2-c, 3-d, 4-a
  * **E.** 1-d, 2-c, 3-a, 4-b
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_cluster\_computacao\_de\_alto\_desempenho.pdf; Semana 3/s3\_texto\_base\_grades\_computacionais.pdf; Semana 3/s3\_texto\_base\_computacao\_em\_nuvem.pdf; Semana 3/s3\_texto\_base\_aspectos\_tecnicos\_envolvidos\_na\_construcao\_de\_um\_cluster.pdf
* **Explicação detalhada:** Clusters costumam reunir máquinas próximas; grids agregam recursos heterogêneos geograficamente distribuídos; nuvem oferece recursos sob demanda; Beowulf é cluster de baixo custo com PCs comuns.
* **Prompt para infográfico:** Crie um infográfico comparando cluster, grid, nuvem e Beowulf em objetivos, escala e exemplos.

### S3Q5

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Em clusters, bibliotecas como MPI são importantes porque:

  * **A.** Substituem o hardware de rede.
  * **B.** Permitem comunicação por passagem de mensagens entre processos/nós.
  * **C.** Criam automaticamente qualquer algoritmo paralelo.
  * **D.** Eliminam latência de comunicação.
  * **E.** Impedem uso de Linux.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_aspectos\_tecnicos\_envolvidos\_na\_construcao\_de\_um\_cluster.pdf; Semana 3/s3\_videoaula5.pdf
* **Explicação detalhada:** Em memória distribuída, os nós não compartilham memória diretamente. MPI permite enviar e receber mensagens para coordenar partes do cálculo.
* **Prompt para infográfico:** Crie um infográfico sobre MPI em clusters, mostrando processos enviando mensagens entre nós.

### S3Q6

* **Nível:** Média
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Clusters podem melhorar desempenho. II) Clusters exigem interconexão entre nós. III) Em clusters, comunicação nunca tem custo.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, V
  * **D.** F, V, F
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_cluster\_computacao\_de\_alto\_desempenho.pdf; Semana 3/s3\_videoaula5.pdf
* **Explicação detalhada:** Clusters podem acelerar aplicações, mas dependem de rede/interconexão. A comunicação tem custo e pode limitar desempenho, especialmente em aplicações com muita troca de dados.
* **Prompt para infográfico:** Crie um infográfico sobre desempenho em clusters, destacando processamento, rede, latência e gargalos.

### S3Q7

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** A principal vantagem da computação em grade é:

  * **A.** Integrar recursos distribuídos e heterogêneos para resolver grandes problemas.
  * **B.** Substituir todos os computadores por um único chip.
  * **C.** Exigir que todos os recursos pertençam à mesma sala.
  * **D.** Eliminar autenticação e políticas de uso.
  * **E.** Impedir cooperação entre instituições.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_grades\_computacionais.pdf
* **Explicação detalhada:** Grades computacionais permitem compartilhar recursos de diferentes locais e instituições, coordenando processamento e dados para tarefas científicas ou intensivas.
* **Prompt para infográfico:** Crie um infográfico sobre grid computing com múltiplas instituições compartilhando recursos computacionais.

### S3Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Em um cluster Beowulf, a escolha da rede é crítica porque:

  * **A.** O sistema não usa mensagens.
  * **B.** A rede substitui completamente os processadores.
  * **C.** A comunicação entre nós pode limitar o ganho paralelo.
  * **D.** O desempenho independe da interconexão.
  * **E.** A rede impede balanceamento de carga.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_aspectos\_tecnicos\_envolvidos\_na\_construcao\_de\_um\_cluster.pdf
* **Explicação detalhada:** Em aplicações paralelas distribuídas, parte do tempo é gasto comunicando dados. Redes lentas ou congestionadas aumentam latência e reduzem eficiência.
* **Prompt para infográfico:** Crie um infográfico sobre impacto da rede em clusters Beowulf: latência, largura de banda, mensagens e eficiência.

### S3Q9

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Uma diferença central entre cluster e nuvem é:

  * **A.** Cluster não pode executar tarefas paralelas.
  * **B.** Nuvem nunca usa servidores físicos.
  * **C.** Cluster costuma ser infraestrutura controlada/local; nuvem oferece recursos abstratos e elásticos como serviço.
  * **D.** Nuvem não permite escalabilidade.
  * **E.** Cluster sempre é mundial e heterogêneo.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_cluster\_computacao\_de\_alto\_desempenho.pdf; Semana 3/s3\_texto\_base\_computacao\_em\_nuvem.pdf
* **Explicação detalhada:** Embora ambos usem múltiplos recursos, clusters são frequentemente ambientes dedicados. A nuvem abstrai infraestrutura e oferece elasticidade, provisionamento rápido e modelos de serviço.
* **Prompt para infográfico:** Crie um infográfico comparando cluster local e nuvem: controle, elasticidade, custo, provisionamento e uso típico.

### S3Q10

* **Nível:** Difícil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Virtualização favorece consolidação e elasticidade na nuvem. II) Grid envolve coordenação entre domínios administrativos. III) Cluster Beowulf depende apenas de software, sem hardware de rede.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, F
  * **D.** F, V, V
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 3/s3\_texto\_base\_computacao\_em\_nuvem.pdf; Semana 3/s3\_texto\_base\_grades\_computacionais.pdf; Semana 3/s3\_texto\_base\_aspectos\_tecnicos\_envolvidos\_na\_construcao\_de\_um\_cluster.pdf
* **Explicação detalhada:** Virtualização permite criar recursos flexíveis; grids cruzam domínios administrativos; Beowulf precisa de hardware real, inclusive computadores e rede.
* **Prompt para infográfico:** Crie um infográfico integrando virtualização, grid e Beowulf, destacando o papel de software e hardware.

\---

## Semana 4 — Computação Paralela, OpenMP, CUDA e Criptomoedas

### S4Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** OpenMP é usado principalmente para:

  * **A.** Programação paralela em memória compartilhada por diretivas.
  * **B.** Compactar arquivos PDF.
  * **C.** Criar bancos de dados relacionais.
  * **D.** Enviar mensagens entre empresas.
  * **E.** Substituir placas de vídeo.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_openmp.pdf
* **Explicação detalhada:** OpenMP permite paralelizar programas, especialmente em C/C++ e Fortran, usando diretivas para distribuir trabalho entre threads em sistemas de memória compartilhada.
* **Prompt para infográfico:** Crie um infográfico explicando OpenMP: diretivas, threads, memória compartilhada e exemplo de loop paralelo.

### S4Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** CUDA está associado principalmente a:

  * **A.** Programação paralela em GPUs NVIDIA.
  * **B.** Programação exclusiva para impressoras.
  * **C.** Armazenamento em fita magnética.
  * **D.** Sistemas sem paralelismo.
  * **E.** Protocolos bancários.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_introducao\_a\_cuda.pdf
* **Explicação detalhada:** CUDA é uma plataforma/modelo de programação da NVIDIA para executar computação paralela em GPUs, explorando milhares de threads leves.
* **Prompt para infográfico:** Crie um infográfico sobre CUDA com CPU, GPU, kernels, threads e aplicações paralelas.

### S4Q3

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Mineração de criptomoedas envolve:

  * **A.** Evitar completamente gasto de energia.
  * **B.** Imprimir dinheiro físico.
  * **C.** Criar arquivos PDF.
  * **D.** Desligar todos os computadores da rede.
  * **E.** Realizar cálculos computacionais para validar blocos/transações em certos mecanismos de consenso.
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 4/s4-Mineração de criptomoedas\_ guia simples e rápido - Blog Nubank\_ - \[blog.nubank.com.br].pdf
* **Explicação detalhada:** Em sistemas como prova de trabalho, mineradores executam cálculos para encontrar soluções válidas, contribuindo para validação e segurança da rede, recebendo recompensas quando bem-sucedidos.
* **Prompt para infográfico:** Crie um infográfico simples sobre mineração de criptomoedas: transações, bloco, cálculo, validação e recompensa.

### S4Q4

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Em OpenMP, a diretiva parallel for serve para:

  * **A.** Distribuir iterações de um laço entre múltiplas threads.
  * **B.** Apagar todos os arquivos temporários.
  * **C.** Converter código C em Java.
  * **D.** Impedir execução simultânea.
  * **E.** Criar uma GPU virtual.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_openmp.pdf
* **Explicação detalhada:** A diretiva parallel for cria uma região paralela e divide as iterações de um loop entre threads, reduzindo o tempo quando as iterações são independentes.
* **Prompt para infográfico:** Crie um infográfico mostrando um loop serial sendo dividido por OpenMP entre quatro threads.

### S4Q5

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) OpenMP; 2) CUDA; 3) GPU; 4) Kernel. a) Função executada em paralelo na GPU; b) Diretivas para threads em memória compartilhada; c) Processador massivamente paralelo; d) Plataforma NVIDIA.

  * **A.** 1-d, 2-b, 3-a, 4-c
  * **B.** 1-b, 2-d, 3-c, 4-a
  * **C.** 1-a, 2-c, 3-b, 4-d
  * **D.** 1-c, 2-a, 3-d, 4-b
  * **E.** 1-b, 2-a, 3-d, 4-c
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_openmp.pdf; Semana 4/s4\_texto\_base\_introducao\_a\_cuda.pdf
* **Explicação detalhada:** OpenMP usa diretivas; CUDA é a plataforma da NVIDIA; GPU é hardware paralelo; kernel é função executada em muitos threads na GPU.
* **Prompt para infográfico:** Crie um infográfico comparando OpenMP e CUDA, incluindo CPU, GPU, threads e kernels.

### S4Q6

* **Nível:** Média
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) GPUs são boas para tarefas com muito paralelismo de dados. II) CUDA dispensa transferência de dados entre CPU e GPU. III) OpenMP é comum em memória compartilhada.

  * **A.** F, F, V
  * **B.** V, F, V
  * **C.** V, V, F
  * **D.** F, V, V
  * **E.** V, V, V
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_introducao\_a\_cuda.pdf; Semana 4/s4\_texto\_base\_openmp.pdf
* **Explicação detalhada:** GPUs são eficientes para paralelismo de dados. CUDA geralmente exige gerenciar ou considerar transferências entre memória da CPU e GPU. OpenMP é típico para paralelismo em memória compartilhada.
* **Prompt para infográfico:** Crie um infográfico sobre fluxo CUDA: CPU prepara dados, envia para GPU, executa kernel e recebe resultados.

### S4Q7

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Uma limitação comum de programas paralelos é:

  * **A.** Incompatibilidade com todos os sistemas operacionais.
  * **B.** Impossibilidade de usar qualquer laço.
  * **C.** Obrigação de rodar sem memória.
  * **D.** Ausência de entrada e saída.
  * **E.** Overhead de comunicação e sincronização.
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 4/s4\_texto-base\_introducao\_a\_computacao\_paralela.pdf
* **Explicação detalhada:** Paralelizar cria custos adicionais: criar threads, sincronizar, comunicar dados e lidar com dependências. Esses custos podem reduzir ou anular ganhos.
* **Prompt para infográfico:** Crie um infográfico sobre overhead paralelo: criação de threads, comunicação, sincronização e gargalos.

### S4Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Uma aplicação ideal para CUDA tende a ter:

  * **A.** Muitas operações similares sobre grandes volumes de dados independentes.
  * **B.** Uma única operação sequencial com forte dependência entre passos.
  * **C.** Pouquíssimos dados e muitas chamadas bloqueantes de E/S.
  * **D.** Código impossível de dividir.
  * **E.** Necessidade de apenas um thread.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_introducao\_a\_cuda.pdf; Semana 4/s4\_videoaula10.pdf
* **Explicação detalhada:** GPUs brilham quando há paralelismo massivo de dados, com muitos elementos processados por operações semelhantes, como matrizes, imagens, simulações e mineração.
* **Prompt para infográfico:** Crie um infográfico mostrando exemplos ideais e ruins para CUDA, destacando paralelismo de dados.

### S4Q9

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Em mineração por prova de trabalho, o paralelismo é útil porque:

  * **A.** O algoritmo proíbe GPUs.
  * **B.** Cada tentativa precisa esperar todas as anteriores.
  * **C.** Muitas tentativas independentes podem ser testadas simultaneamente.
  * **D.** Não há cálculo envolvido.
  * **E.** A rede não valida blocos.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 4/s4-Mineração de criptomoedas\_ guia simples e rápido - Blog Nubank\_ - \[blog.nubank.com.br].pdf; Semana 4/s4\_texto\_base\_introducao\_a\_cuda.pdf
* **Explicação detalhada:** A busca por um hash válido envolve testar muitos valores. Como as tentativas são em grande parte independentes, hardware paralelo pode acelerar a exploração do espaço de busca.
* **Prompt para infográfico:** Crie um infográfico sobre prova de trabalho mostrando várias tentativas de hash em paralelo até encontrar um valor válido.

### S4Q10

* **Nível:** Difícil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) OpenMP é mais natural em memória compartilhada. II) CUDA exige pensar na hierarquia de memória da GPU. III) Paralelismo sempre gera speedup linear perfeito.

  * **A.** V, V, F
  * **B.** V, V, V
  * **C.** V, F, F
  * **D.** F, V, V
  * **E.** F, F, F
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 4/s4\_texto\_base\_openmp.pdf; Semana 4/s4\_texto\_base\_introducao\_a\_cuda.pdf; Semana 4/s4\_texto-base\_introducao\_a\_computacao\_paralela.pdf
* **Explicação detalhada:** OpenMP trabalha bem com threads em memória compartilhada; CUDA exige considerar memória global, compartilhada e registradores; speedup linear perfeito é raro por overheads, partes seriais e comunicação.
* **Prompt para infográfico:** Crie um infográfico explicando por que speedup paralelo raramente é perfeito, usando OpenMP/CUDA como exemplos.

\---

## Semana 5 — Mensageria, Pub/Sub, Kafka, Hadoop, Spark, IoT e Pix

### S5Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Mensageria em sistemas distribuídos serve para:

  * **A.** Permitir comunicação assíncrona entre componentes.
  * **B.** Apagar mensagens automaticamente antes de serem lidas.
  * **C.** Substituir todos os bancos de dados.
  * **D.** Impedir desacoplamento.
  * **E.** Rodar apenas sem rede.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 5/s5-Por que você deveria utilizar mensageria na sua aplicação - Dinamiz.pdf
* **Explicação detalhada:** Mensageria permite que produtores enviem mensagens para filas ou tópicos, e consumidores processem depois, reduzindo acoplamento e aumentando resiliência.
* **Prompt para infográfico:** Crie um infográfico sobre mensageria com produtor, fila/tópico, consumidor, desacoplamento e processamento assíncrono.

### S5Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** No padrão publish-subscribe:

  * **A.** Não existem consumidores.
  * **B.** Todos os componentes precisam conhecer diretamente todos os destinatários.
  * **C.** Publicadores enviam eventos para tópicos, e assinantes recebem os eventos de interesse.
  * **D.** Mensagens são sempre processadas por um único servidor local.
  * **E.** O padrão impede escalabilidade.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 5/s5-Padrão de Publisher-Subscriber - Azure Architecture Center - Microsoft.pdf
* **Explicação detalhada:** Pub/Sub desacopla produtores e consumidores por meio de tópicos/canais. Quem publica não precisa saber quem receberá; assinantes escolhem os tópicos relevantes.
* **Prompt para infográfico:** Crie um infográfico do padrão Pub/Sub com publicadores, tópico e múltiplos assinantes.

### S5Q3

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Apache Kafka é conhecido como:

  * **A.** Editor de imagens.
  * **B.** Plataforma distribuída de streaming/eventos baseada em tópicos e logs.
  * **C.** Sistema operacional móvel.
  * **D.** Linguagem de programação funcional.
  * **E.** Driver de impressora.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 5/s5-O que é Apache Kafka.pdf; Semana 5/s5-Uma introdução ao Apache Kafka, lições aprendidas em um ambiente.pdf
* **Explicação detalhada:** Kafka armazena eventos em tópicos particionados e permite publicação, assinatura, retenção e processamento de fluxos em alta escala.
* **Prompt para infográfico:** Crie um infográfico sobre Kafka com produtores, brokers, tópicos, partições, consumidores e retenção de eventos.

### S5Q4

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) Produtor; 2) Consumidor; 3) Broker; 4) Tópico. a) Recebe/processa mensagens; b) Envia mensagens; c) Intermediário/servidor; d) Canal lógico de eventos.

  * **A.** 1-b, 2-c, 3-a, 4-d
  * **B.** 1-a, 2-b, 3-d, 4-c
  * **C.** 1-c, 2-d, 3-a, 4-b
  * **D.** 1-d, 2-c, 3-b, 4-a
  * **E.** 1-b, 2-a, 3-c, 4-d
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 5/s5-Padrão de Publisher-Subscriber - Azure Architecture Center - Microsoft.pdf; Semana 5/s5-O que é Apache Kafka.pdf
* **Explicação detalhada:** Produtores publicam mensagens; consumidores leem; brokers intermedeiam e armazenam; tópicos organizam fluxos de eventos.
* **Prompt para infográfico:** Crie um infográfico com os papéis de produtor, consumidor, broker e tópico em uma arquitetura de mensageria.

### S5Q5

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Hadoop é associado principalmente a:

  * **A.** Substituição de todos os sistemas de arquivos locais por PDF.
  * **B.** Renderização 3D em navegador.
  * **C.** Mineração exclusiva de criptomoedas.
  * **D.** Armazenamento e processamento distribuído de grandes volumes de dados.
  * **E.** Comunicação Bluetooth.
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 5/s5\_texto\_base\_apache\_hadoop.pdf
* **Explicação detalhada:** Hadoop inclui HDFS para armazenamento distribuído e MapReduce/ecossistema para processamento de grandes dados em clusters.
* **Prompt para infográfico:** Crie um infográfico sobre Hadoop com HDFS, blocos, nós, replicação e processamento distribuído.

### S5Q6

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Apache Spark diferencia-se por:

  * **A.** Ser apenas um editor de texto.
  * **B.** Processamento distribuído rápido, frequentemente em memória, para batch e streaming.
  * **C.** Exigir que todos os dados caibam em uma planilha local.
  * **D.** Não executar em clusters.
  * **E.** Eliminar completamente programação.
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 5/s5\_texto\_base\_apache\_spark.pdf
* **Explicação detalhada:** Spark é uma engine distribuída para processamento de dados, com APIs de alto nível, execução em memória e suporte a SQL, streaming, machine learning e grafos.
* **Prompt para infográfico:** Crie um infográfico comparando Hadoop/MapReduce e Spark, destacando processamento em memória e casos de uso.

### S5Q7

* **Nível:** Média
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) IoT pode gerar fluxos contínuos de dados. II) ThingSpeak é usado para coletar/visualizar dados IoT. III) Sistemas de mensageria são inúteis em IoT.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, V
  * **D.** F, V, F
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 5/s5-Learn More - ThingSpeak IoT.pdf
* **Explicação detalhada:** Dispositivos IoT geram eventos e leituras continuamente. Plataformas como ThingSpeak ajudam a coletar e visualizar dados. Mensageria é útil para transportar eventos de sensores.
* **Prompt para infográfico:** Crie um infográfico sobre fluxo IoT: sensor, rede, plataforma ThingSpeak, visualização e alertas.

### S5Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Partições em Kafka ajudam porque:

  * **A.** Permitem paralelismo, escalabilidade e distribuição dos dados de um tópico.
  * **B.** Impedem múltiplos consumidores.
  * **C.** Apagam automaticamente todos os eventos.
  * **D.** Eliminam necessidade de brokers.
  * **E.** Transformam eventos em arquivos PDF.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 5/s5-O que é Apache Kafka.pdf; Semana 5/s5-Uma introdução ao Apache Kafka, lições aprendidas em um ambiente.pdf
* **Explicação detalhada:** Um tópico pode ser dividido em partições distribuídas entre brokers. Isso permite maior vazão, paralelismo de consumo e tolerância a falhas quando combinado com replicação.
* **Prompt para infográfico:** Crie um infográfico detalhando tópicos, partições, brokers e grupos de consumidores no Kafka.

### S5Q9

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** A rápida aceitação do Pix está relacionada, entre outros fatores, a:

  * **A.** Ausência de sistemas distribuídos.
  * **B.** Funcionamento apenas em horário bancário.
  * **C.** Infraestrutura digital, disponibilidade, integração bancária e experiência de uso simples.
  * **D.** Proibição de APIs.
  * **E.** Processamento manual de todas as transações.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 5/s5-A magia por trás do Pix - Revista IstoÉ Dinheiro.pdf; Semana 5/s5-Como a tecnologia de ponta contribuiu para a rápida aceitação do Pix.pdf; Semana 5/s5-rh-central-bank-of-brazil-case-study-f26354pr-202012-a4-ptbr.pdf
* **Explicação detalhada:** O Pix depende de infraestrutura confiável, interoperabilidade entre instituições, disponibilidade quase contínua, baixa fricção para usuários e integração com sistemas financeiros.
* **Prompt para infográfico:** Crie um infográfico sobre arquitetura conceitual do Pix: usuário, instituição financeira, infraestrutura central, liquidação, disponibilidade e adoção.

### S5Q10

* **Nível:** Difícil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Pub/Sub reduz acoplamento temporal e espacial. II) Kafka pode reter eventos para consumo posterior. III) Spark e Hadoop não têm relação com big data.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, F
  * **D.** F, V, V
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 5/s5-Padrão de Publisher-Subscriber - Azure Architecture Center - Microsoft.pdf; Semana 5/s5-O que é Apache Kafka.pdf; Semana 5/s5\_texto\_base\_apache\_hadoop.pdf; Semana 5/s5\_texto\_base\_apache\_spark.pdf
* **Explicação detalhada:** Pub/Sub desacopla produtores e consumidores; Kafka mantém logs/eventos por política de retenção; Hadoop e Spark são tecnologias centrais em big data.
* **Prompt para infográfico:** Crie um infográfico integrando Pub/Sub, Kafka, Hadoop e Spark em uma arquitetura de dados moderna.

\---

## Semana 6 — Avaliação de Desempenho, Testes de Carga/Estresse e JMeter

### S6Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Teste de carga avalia:

  * **A.** O comportamento do sistema sob uma carga esperada ou planejada.
  * **B.** Apenas a cor da interface.
  * **C.** A qualidade gramatical do código.
  * **D.** O número de arquivos PDF.
  * **E.** A temperatura ambiente.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 6/s6-Testes de estresse e carga\_ conheça os tipos e ferramentas - Prime.pdf; Semana 6/s6-Teste de performance com JMeter - DevMedia.pdf
* **Explicação detalhada:** Teste de carga mede como o sistema responde quando submetido a volumes previstos de usuários, requisições ou transações.
* **Prompt para infográfico:** Crie um infográfico sobre teste de carga com usuários virtuais, requisições, tempo de resposta e throughput.

### S6Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Teste de estresse busca:

  * **A.** Executar apenas um usuário por vez.
  * **B.** Garantir que o sistema nunca falhe.
  * **C.** Identificar limites e comportamento do sistema além da carga normal.
  * **D.** Testar exclusivamente layout.
  * **E.** Medir somente espaço em disco.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 6/s6-Testes de estresse e carga\_ conheça os tipos e ferramentas - Prime.pdf
* **Explicação detalhada:** Teste de estresse aumenta a carga até ultrapassar condições normais, observando degradação, falhas, recuperação e capacidade limite.
* **Prompt para infográfico:** Crie um infográfico comparando teste de carga e teste de estresse, com curva de carga versus desempenho.

### S6Q3

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Apache JMeter é usado para:

  * **A.** Criar circuitos eletrônicos.
  * **B.** Editar vídeos.
  * **C.** Testes de performance/carga em aplicações e serviços.
  * **D.** Desenvolver sistemas operacionais.
  * **E.** Minerar criptomoedas obrigatoriamente.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 6/s6-Teste de performance com JMeter - DevMedia.pdf
* **Explicação detalhada:** JMeter permite simular usuários, criar planos de teste, enviar requisições HTTP/API e coletar métricas de desempenho.
* **Prompt para infográfico:** Crie um infográfico do JMeter: plano de teste, grupo de threads, sampler, listeners e métricas.

### S6Q4

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Throughput representa:

  * **A.** Quantidade de operações/requisições processadas por unidade de tempo.
  * **B.** Tempo que a tela fica azul.
  * **C.** Tamanho da fonte da aplicação.
  * **D.** Número de linhas de código comentadas.
  * **E.** Quantidade de usuários cadastrados historicamente.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 6/s6\_texto\_base\_SSC0643\_e\_SSC5872.pdf; Semana 6/s6\_videoaula15.pdf
* **Explicação detalhada:** Throughput mede vazão, como requisições por segundo. É uma métrica essencial para avaliar capacidade de processamento.
* **Prompt para infográfico:** Crie um infográfico sobre métricas de performance: throughput, latência, tempo de resposta e taxa de erro.

### S6Q5

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) Latência; 2) Tempo de resposta; 3) Throughput; 4) Taxa de erro. a) Falhas por total; b) Operações por tempo; c) Atraso de comunicação/processamento; d) Tempo até concluir requisição.

  * **A.** 1-b, 2-a, 3-d, 4-c
  * **B.** 1-a, 2-b, 3-c, 4-d
  * **C.** 1-d, 2-c, 3-a, 4-b
  * **D.** 1-c, 2-d, 3-b, 4-a
  * **E.** 1-c, 2-a, 3-d, 4-b
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 6/s6\_texto\_base\_SSC0643\_e\_SSC5872.pdf; Semana 6/s6\_videoaula15.pdf
* **Explicação detalhada:** Latência é atraso; tempo de resposta inclui o ciclo da requisição; throughput mede vazão; taxa de erro mede proporção de falhas.
* **Prompt para infográfico:** Crie um infográfico associando as principais métricas de performance a exemplos práticos.

### S6Q6

* **Nível:** Média
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Testes devem ter cenário e carga bem definidos. II) Resultados de performance dependem do ambiente. III) Uma única execução sempre prova estabilidade definitiva.

  * **A.** V, V, V
  * **B.** V, F, V
  * **C.** V, V, F
  * **D.** F, V, F
  * **E.** F, F, F
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 6/s6-Teste de performance com JMeter - DevMedia.pdf; Semana 6/s6-Testes de estresse e carga\_ conheça os tipos e ferramentas - Prime.pdf
* **Explicação detalhada:** Testes precisam de planejamento, massa de dados, carga e ambiente controlados. Uma única execução não garante estabilidade; é necessário repetir e analisar variação.
* **Prompt para infográfico:** Crie um infográfico com boas práticas para testes de performance: cenário, ambiente, repetição, métricas e análise.

### S6Q7

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Um gargalo de desempenho é:

  * **A.** Um componente que limita a capacidade global do sistema.
  * **B.** Um recurso que sempre sobra.
  * **C.** Um tipo de arquivo.
  * **D.** Uma métrica sem relação com performance.
  * **E.** Um erro exclusivo de interface.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 6/s6\_texto\_base\_SSC0643\_e\_SSC5872.pdf; Semana 6/s6\_videoaula16.pdf
* **Explicação detalhada:** Gargalos podem ocorrer em CPU, memória, disco, rede, banco de dados ou código. O desempenho total fica limitado pelo componente mais restritivo.
* **Prompt para infográfico:** Crie um infográfico sobre gargalos de desempenho com exemplos em CPU, memória, disco, rede e banco.

### S6Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Em JMeter, um Thread Group representa:

  * **A.** Conjunto de usuários virtuais, com configuração de quantidade, ramp-up e repetições.
  * **B.** Uma tabela de banco de dados.
  * **C.** Um arquivo de log do sistema operacional.
  * **D.** Um plugin gráfico obrigatório.
  * **E.** Uma thread real única e fixa do servidor.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 6/s6-Teste de performance com JMeter - DevMedia.pdf
* **Explicação detalhada:** O Thread Group define quantos usuários virtuais serão simulados, como eles entram no teste e quantas vezes executam o plano.
* **Prompt para infográfico:** Crie um infográfico explicando Thread Group no JMeter: usuários virtuais, ramp-up, loops e carga gerada.

### S6Q9

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Se o tempo de resposta aumenta muito enquanto o throughput estabiliza, isso pode indicar:

  * **A.** Que a rede foi removida.
  * **B.** Melhoria linear perfeita.
  * **C.** Ausência de carga.
  * **D.** Que não há usuários usando o sistema.
  * **E.** Saturação/gargalo em algum recurso do sistema.
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 6/s6\_texto\_base\_SSC0643\_e\_SSC5872.pdf; Semana 6/s6\_videoaula17.pdf
* **Explicação detalhada:** Quando a carga cresce e o sistema não aumenta a vazão, as requisições começam a enfileirar, elevando tempo de resposta. Isso indica saturação de algum recurso.
* **Prompt para infográfico:** Crie um infográfico com gráfico carga x throughput x tempo de resposta, mostrando ponto de saturação.

### S6Q10

* **Nível:** Difícil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Teste de pico avalia aumentos súbitos de carga. II) Teste de endurance observa comportamento por longo período. III) Teste de performance deve ignorar taxa de erro.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, F
  * **D.** F, V, V
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 6/s6-Testes de estresse e carga\_ conheça os tipos e ferramentas - Prime.pdf; Semana 6/s6\_videoaula18.pdf
* **Explicação detalhada:** Teste de pico verifica resposta a aumentos repentinos; endurance/soak test observa estabilidade ao longo do tempo; taxa de erro é métrica essencial.
* **Prompt para infográfico:** Crie um infográfico sobre tipos de testes de performance: carga, estresse, pico e endurance.

\---

## Semana 7 — Docker, Microserviços, OpenShift e Kubernetes

### S7Q1

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Docker é usado principalmente para:

  * **A.** Criar hardware físico.
  * **B.** Editar imagens manualmente.
  * **C.** Substituir toda a Internet.
  * **D.** Criar e executar aplicações em contêineres.
  * **E.** Eliminar dependências de software sem empacotá-las.
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 7/s7\_revisitando\_conhecimentos\_docker\_e\_sua\_relacao\_com\_microservicos.pdf
* **Explicação detalhada:** Docker empacota aplicação e dependências em contêineres, facilitando portabilidade, isolamento e implantação consistente.
* **Prompt para infográfico:** Crie um infográfico sobre Docker: imagem, contêiner, dependências, portabilidade e isolamento.

### S7Q2

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** Microserviços são:

  * **A.** Serviços que não se comunicam nunca.
  * **B.** Um único programa monolítico obrigatório.
  * **C.** Arquivos PDF executáveis.
  * **D.** Pequenos serviços independentes que compõem uma aplicação maior.
  * **E.** Apenas scripts sem rede.
* **Gabarito:** D
* **Fonte(s) PDF:** Semana 7/s7\_revisitando\_conhecimentos\_docker\_e\_sua\_relacao\_com\_microservicos.pdf
* **Explicação detalhada:** Microserviços dividem uma aplicação em serviços menores, independentes, implantáveis separadamente e comunicando-se por APIs/mensagens.
* **Prompt para infográfico:** Crie um infográfico comparando monólito e microserviços, com serviços independentes e comunicação por API.

### S7Q3

* **Nível:** Fácil
* **Tipo:** Múltipla escolha
* **Enunciado:** OpenShift é:

  * **A.** Plataforma de contêineres baseada em Kubernetes, com recursos corporativos.
  * **B.** Um editor de planilhas.
  * **C.** Um banco de dados relacional obrigatório.
  * **D.** Uma linguagem de programação.
  * **E.** Uma placa de rede.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 7/s7-Red Hat OpenShift.pdf; Semana 7/s7-Introdução ao Red Hat OpenShift no Azure - Azure Red Hat OpenShift.pdf
* **Explicação detalhada:** Red Hat OpenShift é uma plataforma para desenvolver, implantar e operar aplicações em contêineres, construída sobre Kubernetes e adicionando ferramentas de segurança, builds, rotas e gestão.
* **Prompt para infográfico:** Crie um infográfico sobre OpenShift: Kubernetes, contêineres, builds, deploy, rotas e segurança.

### S7Q4

* **Nível:** Média
* **Tipo:** Associação
* **Enunciado:** Associe: 1) Imagem; 2) Contêiner; 3) Pod; 4) Route/Ingress. a) Instância em execução; b) Modelo empacotado; c) Exposição de serviço; d) Unidade básica que agrupa contêineres no Kubernetes.

  * **A.** 1-c, 2-d, 3-a, 4-b
  * **B.** 1-a, 2-b, 3-c, 4-d
  * **C.** 1-b, 2-a, 3-d, 4-c
  * **D.** 1-d, 2-c, 3-b, 4-a
  * **E.** 1-b, 2-c, 3-a, 4-d
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 7/s7\_revisitando\_conhecimentos\_docker\_e\_sua\_relacao\_com\_microservicos.pdf; Semana 7/s7-Red Hat OpenShift.pdf
* **Explicação detalhada:** Imagem é o pacote; contêiner é sua execução; pod é a unidade Kubernetes que hospeda contêineres; route/ingress expõe serviços para acesso externo.
* **Prompt para infográfico:** Crie um infográfico explicando imagem, contêiner, pod e route/ingress em Docker/Kubernetes/OpenShift.

### S7Q5

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Kubernetes/OpenShift ajudam em microserviços porque:

  * **A.** Automatizam implantação, escalonamento, recuperação e exposição de contêineres.
  * **B.** Proíbem múltiplos serviços.
  * **C.** Exigem implantação manual em cada máquina.
  * **D.** Não monitoram estado desejado.
  * **E.** Funcionam apenas sem rede.
* **Gabarito:** A
* **Fonte(s) PDF:** Semana 7/s7-Red Hat OpenShift.pdf; Semana 7/S7-Red Hat OpenShift 4\_ O que há de novo e como criar cluster.pdf
* **Explicação detalhada:** Orquestradores mantêm o estado desejado, reiniciam contêineres com falha, escalam réplicas e gerenciam serviços e rede.
* **Prompt para infográfico:** Crie um infográfico sobre orquestração: deploy, escala, health check, autosserviço e recuperação automática.

### S7Q6

* **Nível:** Média
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) Contêineres compartilham o kernel do host. II) VMs incluem sistema operacional convidado completo. III) Contêineres e VMs são exatamente iguais.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, V
  * **D.** F, V, F
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 7/s7\_revisitando\_conhecimentos\_docker\_e\_sua\_relacao\_com\_microservicos.pdf
* **Explicação detalhada:** Contêineres compartilham o kernel e isolam processos; VMs virtualizam hardware e executam sistemas convidados completos. São tecnologias relacionadas, mas diferentes.
* **Prompt para infográfico:** Crie um infográfico comparando contêineres e máquinas virtuais: kernel, isolamento, peso e tempo de inicialização.

### S7Q7

* **Nível:** Média
* **Tipo:** Múltipla escolha
* **Enunciado:** Um benefício de usar imagens de contêiner é:

  * **A.** Eliminar necessidade de rede em microserviços.
  * **B.** Garantir que bugs nunca ocorram.
  * **C.** Reprodutibilidade do ambiente entre desenvolvimento, teste e produção.
  * **D.** Transformar código em hardware.
  * **E.** Impedir versionamento.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 7/s7\_revisitando\_conhecimentos\_docker\_e\_sua\_relacao\_com\_microservicos.pdf
* **Explicação detalhada:** A imagem empacota dependências e configuração, reduzindo diferenças entre ambientes e facilitando implantação consistente.
* **Prompt para infográfico:** Crie um infográfico sobre ciclo de vida de imagem de contêiner: build, tag, registry, pull e run.

### S7Q8

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** Em OpenShift, um cluster normalmente envolve:

  * **A.** Apenas um navegador web sem backend.
  * **B.** Um único arquivo de texto sem servidores.
  * **C.** Nós de controle e nós de trabalho executando cargas em contêineres.
  * **D.** Ausência de rede entre nós.
  * **E.** Proibição de imagens.
* **Gabarito:** C
* **Fonte(s) PDF:** Semana 7/S7-Red Hat OpenShift 4\_ O que há de novo e como criar cluster.pdf; Semana 7/s7-Introdução ao Red Hat OpenShift no Azure - Azure Red Hat OpenShift.pdf
* **Explicação detalhada:** Um cluster Kubernetes/OpenShift possui plano de controle para orquestração e nós de trabalho onde pods/contêineres são executados.
* **Prompt para infográfico:** Crie um infográfico da arquitetura de um cluster OpenShift: control plane, worker nodes, pods, registry, rotas e operadores.

### S7Q9

* **Nível:** Difícil
* **Tipo:** Múltipla escolha
* **Enunciado:** A relação entre Docker e microserviços é forte porque:

  * **A.** Docker substitui APIs.
  * **B.** Docker obriga toda aplicação a ser monolítica.
  * **C.** Microserviços não precisam de implantação.
  * **D.** Contêineres impedem escalabilidade horizontal.
  * **E.** Contêineres facilitam empacotar, isolar e implantar cada serviço independentemente.
* **Gabarito:** E
* **Fonte(s) PDF:** Semana 7/s7\_revisitando\_conhecimentos\_docker\_e\_sua\_relacao\_com\_microservicos.pdf
* **Explicação detalhada:** Cada microserviço pode ser empacotado em sua própria imagem, implantado separadamente, escalado conforme demanda e atualizado com menor impacto no restante do sistema.
* **Prompt para infográfico:** Crie um infográfico mostrando uma aplicação de microserviços com cada serviço em seu contêiner, escalado independentemente.

### S7Q10

* **Nível:** Difícil
* **Tipo:** V/F com alternativas A–E
* **Enunciado:** I) OpenShift adiciona recursos corporativos ao Kubernetes. II) Deployments ajudam a manter réplicas desejadas. III) Orquestração elimina a necessidade de observabilidade.

  * **A.** V, V, V
  * **B.** V, V, F
  * **C.** V, F, F
  * **D.** F, V, V
  * **E.** F, F, F
* **Gabarito:** B
* **Fonte(s) PDF:** Semana 7/s7-Red Hat OpenShift.pdf; Semana 7/S7-Red Hat OpenShift 4\_ O que há de novo e como criar cluster.pdf
* **Explicação detalhada:** OpenShift amplia Kubernetes com ferramentas integradas. Deployments/DeploymentConfigs ajudam a manter estado desejado. Observabilidade continua necessária para monitorar saúde, desempenho e falhas.
* **Prompt para infográfico:** Crie um infográfico sobre operação de aplicações no OpenShift: deployment, réplicas, health checks, logs, métricas e observabilidade.

