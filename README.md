# Repositório SQL do Azure Data
Este repositório do GitHub contém exemplos de código que demonstram como usar os produtos de dados do Azure da Microsoft, incluindo SQL Server, banco de dados SQL do Azure, Azure Synapse e Azure SQL Edge. Cada amostra inclui um arquivo README que explica como executar e usar a amostra.

Observe que determinados recursos, como OLTP na memória, são edições específicas do SQL Server e seriam possíveis de implementar se a edição que dá suporte a esse recurso estiver sendo usada para executar a amostra.

## Lançamentos neste repositório

Os lançamentos permitem que você baixe convenientemente bancos de dados ou aplicativos de amostra sem a necessidade de criá-los a partir do código-fonte. Este repositório de amostras do SQL Server tem os seguintes lançamentos notáveis:

   - [Wide World Importers sample database v1.0](https://github.com/Microsoft/sql-server-samples/releases/tag/wide-world-importers-v1.0) é o principal exemplo do SQL Server 2016 e Banco de Dados SQL do Azure. Ele contém um banco de dados OLTP e OLAP.
   - [In-Memory OLTP Performance Demo v1.0](https://github.com/Microsoft/sql-server-samples/releases/tag/in-memory-oltp-demo-v1.0) ilustra os benefícios de desempenho de a tecnologia OLTP In-Memory integrada ao SQL Server e ao Banco de Dados SQL do Azure.
   - [IoT Smart Grid sample v1.0](https://github.com/Microsoft/sql-server-samples/releases/tag/iot-smart-grid-v1.0) ilustra como o SQL Server pode ser aproveitado para ingerir dados de dispositivos e sensores IoT e como você pode executar análises nesses dados.

Para ver a lista completa de recursos neste repositório, navegue até [Releases](https://github.com/Microsoft/sql-server-samples/releases)

## Trabalhando no GitHub
Para trabalhar no GitHub, acesse https://github.com/microsoft/sql-server-samples e bifurque o repositório. Trabalhe em seu próprio fork e, quando estiver pronto para enviar para fazer uma alteração ou publicar sua amostra pela primeira vez, envie uma solicitação pull para a ramificação master de sql-server-samples. Um dos aprovadores revisará sua solicitação e aceitará ou rejeitará a solicitação pull.

Cada amostra deve estar em sua própria pasta com um arquivo README.md que segue o [template](README_samples_template.md). Arquivos gerados (por exemplo, .exe ou .bacpac) e definições de configuração do usuário (por exemplo, .user) não devem ser confirmados no GitHub.

## Clonando apenas um subconjunto do repositório (com checkout esparso)
Você pode seguir as etapas abaixo para clonar arquivos individuais do repositório git sql-server-samples. Observação: o script a seguir clona apenas os arquivos nas pastas **features** e **demos**.
```
git clone -n https://github.com/daniloopinheiro/RepositorioSQLAzureData
cd RepositorioSQLAzureData
git config core.sparsecheckout true
amostras de eco/recursos/*| out-file -append -encoding ascii .git/info/sparse-checkout
echo RepositorioSQLAzureData/demos/*| out-file -append -encoding ascii .git/info/sparse-checkout
git check-out
```
Para obter mais informações sobre checkout esparso, visite [this](https://stackoverflow.com/questions/23289006/on-windows-git-error-sparse-checkout-leaves-no-entry-on-the-working-directory) thread stackoverflow.

## Código de Conduta
Este projeto adotou o [Código de conduta de código aberto da Microsoft](https://opensource.microsoft.com/codeofconduct/). Para obter mais informações, consulte as [Perguntas freqüentes sobre o Código de Conduta](https://opensource.microsoft.com/codeofconduct/faq/) ou entre em contato com [opencode@microsoft.com](mailto:opencode@microsoft.com) com quaisquer perguntas adicionais ou comentários.

## Licença
Essas amostras e modelos são todos licenciados sob a licença MIT. Consulte o arquivo license.txt na raiz.

## Questões
Envie perguntas por e-mail para: sqlserversamples@microsoft.com.
