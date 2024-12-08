- Descrição do Projeto
  Este programa em Go é uma aplicação para realizar downloads de arquivos da internet, com suporte para:

  I. Retentativa automática: Em caso de falhas no download, são feitas até três tentativas antes de desistir.
  II. Monitoramento de progresso: O progresso do download é exibido em tempo real para o usuário.
  III. Criação de estrutura de diretórios: Os arquivos são salvos em uma pasta chamada instalados, que é criada automaticamente caso não exista.
  IV. Validação de arquivos existentes: Se o arquivo já existe no destino, o download é ignorado.

- Funcionalidades
  Entrada de dados do usuário:
  O usuário fornece a URL do arquivo e o nome desejado para salvá-lo.
  
  Gestão do download:
  O programa verifica se o arquivo já foi baixado antes de iniciar o download.
  Caso falhe, são feitas tentativas automáticas com intervalo de 2 segundos entre elas.
  
  Exibição de progresso:
  Durante o download, o progresso é calculado e exibido em porcentagem.
  
  Estrutura organizada:
  Todos os arquivos baixados são armazenados na pasta instalados.

- Pré-requisitos
  Para executar o programa, você precisará de:

  I. Go instalado na sua máquina (versão 1.16 ou superior recomendada).
  II. Conexão com a internet para realizar os downloads.

- Como Executar
  
  I. Clone o repositório (se aplicável) ou copie o código para um arquivo local.
  II. Salve o arquivo com o nome main.go.
  III. No terminal, navegue até o diretório onde o arquivo foi salvo e execute o comando **go run main.go**.
  IV. Insira os dados solicitados:
    A URL do arquivo para download.
    O nome com o qual deseja salvar o arquivo.
  V. O programa exibirá mensagens no terminal indicando o progresso e o status final do download.

- Estrutura de Arquivos

  **instalados/
    └── <arquivo_baixado>
  main.go**
  A pasta instalados será criada automaticamente no mesmo diretório onde o programa está sendo executado.

