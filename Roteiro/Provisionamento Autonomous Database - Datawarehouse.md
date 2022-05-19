# Provisionamento Autonomous Database - Datawarehouse

## Criando uma instância do Autonomous Data Warehouse

Clicar no Hambúrguer superior esquerdo, <i>Oracle Database</i> e <i>Autonomous Data Warehouse</i>
  
![image](https://user-images.githubusercontent.com/46925501/155531068-e823c84f-3210-46b5-8777-121221267337.png)

Verifique se o compartimento está correto e clique em <i>Create Autonomous Database</i>
  
![image](https://user-images.githubusercontent.com/46925501/155531442-d1aab77d-acd2-4d0a-8d2b-85beda0d63dd.png)

Informar as informações de <i>Display Name</i>, <i>Database Name</i>

![image](https://user-images.githubusercontent.com/46925501/155531754-eaa11f9e-abf7-4469-b88b-77de1be498ac.png)

Escolher a opção <i>Data Warehouse</i> em Workload Type e <i>Shared Infrastructure</i> em Deployment Type
  
![image](https://user-images.githubusercontent.com/46925501/155531853-ed62f919-91df-4f71-8c89-f5e74efc0ade.png)

Para fins de laboratório, vamos utilizar o Autonomous na versão free. Habilite a flag conforme abaixo:
  
![image](https://user-images.githubusercontent.com/46925501/155532160-00d419e2-bfc7-464f-adc3-899448ed1cd4.png)

Inserir o password para o usuário ADMIN e após clicar em <i>Create Autonomous Database</i>

![image](https://user-images.githubusercontent.com/46925501/155532347-1a68151d-bc96-4040-b794-a7674cbdd77b.png)

Aguardar o Provisionamento da instância

![image](https://user-images.githubusercontent.com/46925501/155532515-a38c5be1-068d-4914-a8cb-e72d7a3043af.png)

## Criando Database User

Após a criação da instância, clique em <i>Database Actions</i>

![image](https://user-images.githubusercontent.com/46925501/169381881-89d01052-1f34-4e23-8895-7fd14afc5b68.png)

Em <i>Database Actions</i> na sessão <i>Administration</i> clique em <i>Database Users</i>

![image](https://user-images.githubusercontent.com/46925501/169382132-75184f33-2003-4c3e-b886-3e21600f90b8.png)

Na página do <i>Database Users</i>, clique em <i>Create User</i>

![image](https://user-images.githubusercontent.com/46925501/169382231-d8f66cbc-a2d4-4b27-a3b4-1a316904565f.png)

Você irá preencher os campos conforme imagem abaixo - Obs. Lembrando que em <i>User Name</i> você deve colocar o nome do seu usuário

![image](https://user-images.githubusercontent.com/46925501/169382354-97421bcc-a888-453d-b2a0-a5dcbbf28377.png)

Após preencher o formulário acima, clique na aba <i>Grated Roles</i> e adicione o grant conforme imagem e clique em <i>Create User</i>

![image](https://user-images.githubusercontent.com/46925501/169382645-7edb2a57-653c-4bdf-882b-d2d7f4d663bd.png)

Usuário criado com sucesso!
