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

Após as configurações anteriores, teremos um canvas para desenvolvimento do nosso data flow
![image](https://user-images.githubusercontent.com/46925501/169425728-a5da6f45-3289-42e4-9c4e-8ec22ce88804.png)

O primeiro passo é arrastarmos as bases de dados que vamos trabalhar para o cavas. Para isso clique na entidade de dados <i>Movie_SALES_2020</i> e arraste para o canvas; realizar o mesmo para a entidade de dados <i>DEVICES</i>
![image](https://user-images.githubusercontent.com/46925501/169423937-111bac86-c7c1-490a-8af4-355ed84b82d4.png)

Após arrastar as entidades de dados para o canvas, vamos adicionar o operador join. Para isso em <i>DATA TRANSFORM</i> selecionar o operador <i>Join</i> e arrastar para o canvas
![image](https://user-images.githubusercontent.com/46925501/169424173-5299d6ee-83e7-4de3-88f9-ec85a32b0cdb.png)

Agora vamos ligar as entidades de dados ao operador JOIN. Clica na entidade de dados, irá aparecer uma pequena seta, clique nela e arraste até o operador que deseja conectar. Realizar o mesmo processo com a entidade de dados <i>DEVICES</i>
![image](https://user-images.githubusercontent.com/46925501/169424424-ca305ce9-b615-4735-925b-12041f789f0f.png)

Clique no operador <i>JOIN</i> e atribua um nome a ele
![image](https://user-images.githubusercontent.com/46925501/169424640-1680da0d-b354-45a7-a66c-9b8ad93fd1f4.png)

Clique na opção <i>atributtes</i> do operador <i>join</i> e valide se as configurações estão iguais a imagem abaixo
![image](https://user-images.githubusercontent.com/46925501/169424823-f0519abf-57e2-4e1b-9d71-9d3faaf8897f.png)

Agora vamos configurar a tabela de destino dos dados que trabalhamos. Para isso ainda no operador <i>JOIN</i> clique na tabelinha conforme imagem
![image](https://user-images.githubusercontent.com/46925501/169424972-ba244989-6188-4151-81d8-bb07022b0b73.png)

Preencher as informações baseado no formulário abaixo
![image](https://user-images.githubusercontent.com/46925501/169425121-f723d8d6-b07b-420b-bd7b-6e43179813db.png)

Verifique se todas as colunas estão presentes e clique em next
![image](https://user-images.githubusercontent.com/46925501/169425211-a6906227-c96e-4d54-9618-0974636f5652.png)

E por fim, cliquem em salvar.

## Executando nosso Data Flow

Agora que criamos nosso fluxo de dados, vamos salvar e executar
![image](https://user-images.githubusercontent.com/46925501/169425348-e0542ae8-420d-43d9-bafd-49b32778e654.png)

Irá surgir um pop-up e clique em start
![image](https://user-images.githubusercontent.com/46925501/169425454-bfbac2ce-ec25-47ce-9c82-e926e6b9bfcb.png)

Irá aparcer uma mensagem com o job que foi criado para a execução do seu fluxo de dados, clique nele
![image](https://user-images.githubusercontent.com/46925501/169425513-df7c9079-0a06-4fb2-8ca7-26a8409c1d20.png)

Você será direcionado para uma console de acompanhamento do seu job. Aguarde finalizar
![image](https://user-images.githubusercontent.com/46925501/169425593-55a5b2cf-53cc-4235-a3bd-3cf834ec66c4.png)

Após a finalização do JOB, você possui seus dados disponíveis para consumo no Autonomous Datawarehouse.
