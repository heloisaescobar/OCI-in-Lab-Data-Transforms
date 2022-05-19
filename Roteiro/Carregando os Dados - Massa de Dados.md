# Carregando os Dados - Massa de Dados

Após criarmos no usuário, vamos fazer a ingestão dos dados que vamos trabalhar nesse laboratório.

Obs. Caso não tenha criado o usuário, [acessar aqui](https://github.com/heloisaescobar/OCI-in-Lab-Data-Transforms/blob/main/Roteiro/Provisionamento%20Autonomous%20Database%20-%20Datawarehouse.md)

Para fazermos o carregamento dos dados, vamos permanecer em <i>Database Actions</i> e clicar em <i>Data Load</i>

![image](https://user-images.githubusercontent.com/46925501/169383744-7c3ca959-bffe-40c3-bb76-2fa36ef69cfb.png)

Na próxima janela, vamos adicionar um conector com a nossa fonte de dados (Object Storage), para isso selecione <i>Cloud Locations</i>

![image](https://user-images.githubusercontent.com/46925501/169384077-72de039c-90f8-4dd6-a7bb-61db2f900363.png)

Clique em <i>Add Cloud Storage</i>

![image](https://user-images.githubusercontent.com/46925501/169384166-e46ef8a7-2512-4677-a0a8-d328794e9e9a.png)

Preencher formulário conforme imagem e no campo <i>Bucket URI</i> preencher com o link: https://objectstorage.us-ashburn-1.oraclecloud.com/n/id3kyspkytmr/b/bucket-public-evento/o/

![image](https://user-images.githubusercontent.com/46925501/169384378-b46d01e7-8790-4d67-85ee-a4f47680ef7f.png)

Após criarmos nosso conector, vamos realizar a carga dos dados, selecionando <i>Load Data</i> e <i>Cloud Storage</i> conforme imagem

![image](https://user-images.githubusercontent.com/46925501/169384563-b5046e5b-9780-4bdd-9acb-b5ea6e57624c.png)

Teremos uma espaço com todos os arquivos que estão no bucket apontado, para carregarmos esse dado, vamos selecionar o arquivo que queremos carregar para o Autonomous e arrastar para o canvas, conforme imagem.

Obs. Realizar esse procedimento para os arquivos <b><i>Movie_Sales_2020.csv</i></b> e <b><i>Devices.csv<i></b>
![image](https://user-images.githubusercontent.com/46925501/169385566-214a1a75-2d57-4dda-978e-b6add9f53bb1.png)


