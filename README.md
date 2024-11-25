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

Utilizei o ScrollView que é um grupo de visualização que é usado para fazer visualizações roláveis ​​verticalmente .
Para colocar várias visualizações na visualização de rolagem, é preciso fazer um grupo de visualização (como LinearLayout) e então podemos definir muitas visualizações dentro dele.

