# blockytest

Repositório para armazenar os arquivos gerados durante o teste do [blocky](https://gist.github.com/antoniosb/dd79afc4942996fc0b690a459fbbc453)

O código em questão foi compilado e a execução de seu código foi verificada através do uso de [bcc-tools](https://github.com/iovisor/bcc). 


Pelo que verifiquei imagino que a aplicação está constantemente abrindo novas threads que nunca finalizam realizando essa tividade em loop infinito enquanto isso. Enquanto a aplicação rodava executei a ferramenta **profile** que mostrava atividade na cpu e executei o **offcpu* que estava mostrando os tempos do processo em offcpu constantemente aumentando conforme a aplicação ia executando, no final coletei os stacktraces e gerei o **flamegraph**, os arquivos estão em anexo.
