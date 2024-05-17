# Este é um registro detalhado do processo de construção da imagem Docker, que inclui várias etapas:

Inicialização do ambiente: O ambiente do CodeBuild é inicializado e configurado para a execução do processo de construção.

# 1 etapa Fase DOWNLOAD_SOURCE: O código-fonte é baixado para o ambiente de construção. Aqui, o arquivo buildspec.yml é identificado e processado.


# 2 etapa Fase INSTALL: Esta fase não envolve comandos específicos, indicando que não há etapas de instalação adicionais especificadas no arquivo de configuração.


# 3 etapa Fase PRE_BUILD: Nesta fase, são executadas algumas operações preliminares, como a autenticação no Docker Hub e no Amazon ECR. Além disso, algumas variáveis de ambiente são exportadas para uso posterior.


# 4 etapa Fase BUILD: Aqui, a construção real da imagem Docker ocorre. O Dockerfile é processado, resultando em uma imagem Docker. O processo inclui várias etapas, como:

# Preparação do ambiente de construção.
Instalação de dependências do Node.js e Angular CLI.
Configuração do projeto Angular.
Compilação do código-fonte Angular.
Construção da imagem Docker final.
Fase POST_BUILD: Após a construção da imagem, algumas operações pós-construção são realizadas, como marcação e envio da imagem para o Amazon ECR, e a geração de um arquivo de definição de imagem para o ECS.

Essa sequência de comandos e eventos mostra o processo completo de construção de uma imagem Docker para uma aplicação Angular, incluindo a preparação do ambiente, a construção da imagem e as operações pós-construção necessárias para implantar a imagem em um registro de contêiner como o Amazon ECR.





	