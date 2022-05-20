# Desenvolvendo seus fluxos no Data Transforms

## Conectando ao Autonomous Data Warehouse

Após logarmos na console do Data Transform, clicamos em <i>Connections</i> e <i>Create Connection</i>

![image](https://user-images.githubusercontent.com/46925501/169422274-719d06f7-555a-4286-972d-b88e73cf605d.png)

Adicionar um nome na conexão e selecionar o conector Oracle
![image](https://user-images.githubusercontent.com/46925501/169422381-8a45ef30-2e6b-4f72-9f24-97bbee4f523a.png)

Para o próximo passo, será necessário fazer o download da wallet do Autonomous Datawarehouse. Para ver o passo a passo [clique aqui]()

Preencha os demais campos conforme formulário abaixo

![image](https://user-images.githubusercontent.com/46925501/169422643-88fcd884-5bb3-4cd3-8998-98b30451358c.png)

Após realizar a configuração da conexão, vamos importar as entidades de dados do nosso banco de dados autonomous. Para isso clicar em <i>Data Entities</i> e <i>Import Data Entities</i>
![image](https://user-images.githubusercontent.com/46925501/169422760-1115f591-79a5-4298-a68b-6e6dad4879e3.png)

Configurar igual o formulario abaixo e executar o mapeamento das entidades de dados
![image](https://user-images.githubusercontent.com/46925501/169422862-19a4a643-e30d-457d-bb64-5855b3928767.png)

Finalizando o mapeamento das entidades de dados, elas vão aparecer na console similar a imagem abaixo
![image](https://user-images.githubusercontent.com/46925501/169422946-6af0d5fe-c545-4175-9736-9e8a5fb88cf3.png)

## Criando nosso primeiro projeto no Data Transform

Agora vamos iniciar criando nosso primeiro projeto no Data Transforma. Para isso vamos clicar em <i>Projects</i> e <i>Create Data Flow</i>

![image](https://user-images.githubusercontent.com/46925501/169423122-29951aa1-20ac-4c0c-96d2-6bd487692a7b.png)

Preencher o formulário com as informações do projeto conforme imagem abaixo
![image](https://user-images.githubusercontent.com/46925501/169423195-6145ffcb-7480-4422-9064-568a0f23d47d.png)

