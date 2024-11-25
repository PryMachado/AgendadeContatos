Usando Room para Persistência de Dados no Desenvolvimento Android - APP DE LISTA DE CONTATOS 
baseado na documentacao https://developer.android.com/training/data-storage/room?hl=pt-br


O caso de uso mais comum é armazenar em cache partes importantes de dados para que, 
quando o dispositivo não puder acessar a rede, o usuário ainda consiga ter acesso a esse conteúdo off-line.

CONFIGURANDO O COD :

-Adicionar dependências no arquivo build.gradledo módulo
-Em Kotlin, também habilite o KAPT no início do arquivo build.gradle
-Crie uma entidade a@Entity
@Entity: @PrimaryKey:
autoGenerate = true: Faz com que o ID seja gerado automaticamente.

-Criei o DAO (objeto de acesso a dados)
O DAO é uma interface ou classe abstrata onde você define os métodos para interagir com o banco de dados (consultas, inserções, exclusões, etc.).
-@Inserir:D
@Consulta :
@Atualização : Atual
@Excluir:R

-Utlizilei a classe do banco de dados
A classe do banco de dados é uma abstração sobre o banco SQLite. Use uma anotação@Databasepara defini-la.RoomDatabase.
entities:  version:

- Usei tbm o DAO para interagir com o banco
 você pode usar o DAO para realizar operações no banco. -se de realizar essas operações em um fio separado (como em corrotinas).

-Utilizando tbm Toast.makeText

Utilizei o ScrollView que é um grupo de visualização que é usado para fazer visualizações roláveis ​​verticalmente .
Para colocar várias visualizações na visualização de rolagem, é preciso fazer um grupo de visualização (como LinearLayout) e então podemos definir muitas visualizações dentro dele.

-Configurando o Banco de dados 

-Criando o Layout da tela de cadastro

-Salvando dados em um banco de dados Room

-Criando o item da lista e configurando o adapter 

-Listando todos os contatos, Atualizando os dados do usuário e deletando o usuário 
![Screenshot_20241125_012433](https://github.com/user-attachments/assets/4fdafc73-e34c-4864-8fcd-df2de697c0e7) 
![Screenshot_20241125_012502](https://github.com/user-attachments/assets/a3cf424a-6cdc-4298-b35f-f94149570998)
![Screenshot_20241125_012547](https://github.com/user-attachments/assets/9e6a933a-14a5-4591-a8b0-9253bb4ae33a)
![Screenshot_20241125_012601](https://github.com/user-attachments/assets/6deee278-68b7-4308-a7c9-3f2e8f8ddfde)
![Screenshot_20241125_012618](https://github.com/user-attachments/assets/992baf0e-2ce7-45d2-b185-5afe95e1f424)

