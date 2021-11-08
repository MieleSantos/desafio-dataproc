## Desafio GCP Dataproc
## DiogitalInnovation One - Bootcamp Cognizant Cloud Data Engineer

Ministrado por: Marcelo Marques<br>

O desafio faz parte do curso na plataforma da Digital Innovation One: 

__*Criando um ecossistema Hadoop totalmente gerenciado com Google Cloud Platform*__

O desafio consiste em efetuar um processamento de dados utilizando o produto Dataproc do GCP. Esse processamento irá efetuar a contagem das palavras de um livro e informar quantas vezes cada palavra aparece no mesmo.

------

##### O que é `Google Cloud Platform(GCP)`?

É um grupo de soluções e aplicações que ajuda a executar blocos de serviços em nuvem  com elevado desempenho, proteção e rapidez.

A GCP pode funcionar em hardwares próprios de empresas. Os serviços são comercializados sob medida, sendo que você tem a liberdade de contratar apenas os recursos de seu interesse.

É possível aumentar o controle no gerenciamento das operações, bem como obter saídas completas e protegidas para a cloud storage. Isso vale inclusive para armazenamentos customizados às necessidades de cada cliente.

A Google Cloud Platform oferece facilidades para o desenvolvimento de aplicativos.
 
O aplicativo de música Spotify utiliza a GCP para ofertar uma alta disponibilidade a seus usuários. Esse investimento permitiu um suporte informático que reúne atributos como eficácia, agilidade e exatidão de informações.

------

##### O que é `DataProc`?

O Dataproc é um serviço totalmente gerenciado e altamente escalonável para executar o Apache Spark, o Apache Flink, o Presto e mais de 30 ferramentas e frameworks de código aberto. Use o Dataproc para modernização do data lake, ETL e ciência de dados segura, em escala global, totalmente integrada ao Google Cloud e com custos bem menores.

------

##### O que é um `Bucket`?
O recurso Buckets representa um intervalo no Cloud Storage. Há um único namespace global compartilhado por todos os buckets.

Buckets contêm objetos que podem ser acessados pelos seus próprios métodos. 
 - Além da acl propriedade, os Buckets contêm bucketAccessControls , para uso na manipulação refinada dos controles de acesso de um balde existente.

Um intervalo sempre pertence ao grupo de proprietários da equipe do projeto .

##### O que é `PySpark`?

Apache Spark é escrito na linguagem de programação Scala. PySpark foi lançado para apoiar a colaboração do Apache Spark e Python, na verdade é uma API Python para Spark. Além disso, o PySpark ajuda a fazer a interface com conjuntos de dados distribuídos resilientes (RDDs) na linguagem de programação Apache Spark e Python. Isso foi conseguido tirando proveito da biblioteca Py4j. 
PySpark LogoPy4J é uma biblioteca popular que é integrada ao PySpark e permite que o python faça interface dinâmica com objetos JVM.

------

### Etapas do Desafio

1. Criar um bucket no Cloud Storage
1. Atualizar o arquivo ```contador.py``` com o nome do Bucket criado nas linhas que contém ```{SEU_BUCKET}```.
1. Fazer o upload dos arquivos ```contador.py``` e ```livro.txt``` para o bucket criado (instruções abaixo)
    - https://cloud.google.com/storage/docs/uploading-objects

1. Utilizar o código em um cluster Dataproc, executando um Job do tipo PySpark chamando ```gs://{SEU_BUCKET}/contador.py```
1. O Job irá gerar uma pasta no bucket chamada ```resultado```. Dentro dessa pasta o arquivo ```part-00000``` irá conter a lista de palavras e quantas vezes ela é repetida em todo o livro.

------

### Entrega do Resultado

1. Criar um repositório no GitHub.
2. Criar um arquivo chamado ```resultado.txt```. Dentro desse arquivo, colocar as 10 palavras que mais são usadas no livro, de acordo com o resultado do Job.
3. Inserir os arquivo ```resultado.txt``` e ```part-00000``` no repositório e informar na plataforma da Digital Innovation One.

