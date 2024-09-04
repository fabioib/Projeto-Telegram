# Projeto-Telegram

![architecture](https://github.com/user-attachments/assets/89bcbae4-7d9a-4439-9f96-45d9629f848f)

1 - Coleta de Dados: Utilizamos um bot no Telegram para capturar mensagens, que são automaticamente armazenadas em um bucket no AWS S3. Isso assegura a coleta contínua e segura das mensagens enviadas pelos usuários.

2 - Processamento de Dados (ETL): Criamos uma função no AWS Lambda para realizar o processo de ETL (Extract, Transform, Load). Esta etapa inclui a limpeza, transformação e organização das mensagens coletadas, preparando-as para análise.

3 - Acesso via API: Implementamos uma API web no AWS API Gateway para disponibilizar os dados processados. Essa API permite que outros sistemas e aplicações acessem e interajam com as informações do Telegram de forma controlada e segura.

4 - Arquitetura Baseada em Eventos: A infraestrutura foi projetada para operar com eventos, utilizando webhooks da API de bots do Telegram. Isso garante que os sistemas respondam automaticamente a novas mensagens ou eventos no Telegram, proporcionando uma reação rápida e automatizada.

5 - Armazenamento e Análise: Empregamos o AWS Athena para consultar os dados armazenados no S3. Essa abordagem permite consultas SQL rápidas e eficientes sobre os dados do Telegram, eliminando a necessidade de processamento manual extensivo.

Este projeto, integrado com os serviços da AWS, oferece uma solução robusta para a coleta, processamento e disponibilização de dados do Telegram, aproveitando a escalabilidade, segurança e eficiência operacional dos serviços da AWS.
