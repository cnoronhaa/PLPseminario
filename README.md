- Descrição do Projeto
  Este programa em Go é uma aplicação para realizar downloads de arquivos da internet, com suporte para:

  -- Retentativa automática: Em caso de falhas no download, são feitas até três tentativas antes de desistir.
  2. Monitoramento de progresso: O progresso do download é exibido em tempo real para o usuário.
  3. Criação de estrutura de diretórios: Os arquivos são salvos em uma pasta chamada instalados, que é criada automaticamente caso não exista.
  4. Validação de arquivos existentes: Se o arquivo já existe no destino, o download é ignorado.

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

  Go instalado na sua máquina (versão 1.16 ou superior recomendada).
  Conexão com a internet para realizar os downloads.

- Como Executar
  Clone o repositório (se aplicável) ou copie o código para um arquivo local.

  Salve o arquivo com o nome main.go.

  No terminal, navegue até o diretório onde o arquivo foi salvo e execute o comando:

  bash
  Copiar código
  go run main.go
  Insira os dados solicitados:

  A URL do arquivo para download.
  O nome com o qual deseja salvar o arquivo.
  O programa exibirá mensagens no terminal indicando o progresso e o status final do download.

- Estrutura de Arquivos
  plaintext
  Copiar código
  instalados/
    └── <arquivo_baixado>
  main.go
  A pasta instalados será criada automaticamente no mesmo diretório onde o programa está sendo executado.

