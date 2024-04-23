![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)

## Desafio DSMovie Jacoco
Você deve implementar todos os testes unitários de service para o projeto DSMovie.

## Sobre o projeto DSMovie:
Este é um projeto de filmes e avaliações de filmes. A visualização dos dados dos filmes é pública (não necessita login), porém as alterações de filmes (inserir, atualizar, deletar) são permitidas apenas para usuários ADMIN. As avaliações de filmes podem ser registradas por qualquer usuário logado CLIENT ou ADMIN. A entidade Score armazena uma nota de 0 a 5 (score) que cada usuário deu a cada filme. Sempre que um usuário registra uma nota, o sistema calcula a média das notas de todos usuários, e armazena essa nota média (score) na entidade Movie, juntamente com a contagem de votos (count).  Veja vídeo explicativo.

Arquivos de collection e enviroment do Postman estão no projeto.

![image](https://github.com/Sammy192/DSMovie_springExpert/assets/53224915/1605ed6e-d85c-4420-8b20-c0b5c633f829)

Abaixo estão os testes unitários que você deverá implementar. Com todos os testes, o Jacoco deve reportar 100% de cobertura, mas o mínimo para aprovação no desafio são 12 dos 15 testes.

## MovieServiceTests:
  ●	findAllShouldReturnPagedMovieDTO
  
  ●	findByIdShouldReturnMovieDTOWhenIdExists
  
  ●	findByIdShouldThrowResourceNotFoundExceptionWhenIdDoesNotExist
  
  ●	insertShouldReturnMovieDTO
  
  ●	updateShouldReturnMovieDTOWhenIdExists
  
  ●	updateShouldThrowResourceNotFoundExceptionWhenIdDoesNotExist
  
  ●	deleteShouldDoNothingWhenIdExists
  
  ●	deleteShouldThrowResourceNotFoundExceptionWhenIdDoesNotExist
  
  ●	deleteShouldThrowDatabaseExceptionWhenDependentId
  
## ScoreServiceTests:
  ●	saveScoreShouldReturnMovieDTO
  
  ●	saveScoreShouldThrowResourceNotFoundExceptionWhenNonExistingMovieId
  
## UserServiceTests:

  ●	authenticatedShouldReturnUserEntityWhenUserExists
  
  ●	authenticatedShouldThrowUsernameNotFoundExceptionWhenUserDoesNotExists
  
  ●	loadUserByUsernameShouldReturnUserDetailsWhenUserExists
  
  ●	loadUserByUsernameShouldThrowUsernameNotFoundExceptionWhenUserDoesNotExists
  

Implementado testes no projeto e utilizando o Jacoco para cobertura de testes:
●  JaCoCo é uma ferramenta de código aberto (open-source) usada para mensurar a cobertura de código em aplicações;

●  A partir de relatórios visuais é possível identificar as partes do código que estão cobertas e que ainda faltam cobertura;

●  O JaCoCo implementa 3 métricas principais para cobertura, sendo:

 ○  Line Coverage/Statement;
 
 ○  Branch Coverage;
 
Cyclomatic complexity: A partir de uma combinação linear apresenta o números de caminhos que necessitam cobertura.

●  O JaCoCo apresenta auxilia o usuário na visualização e análise da cobertura usando diamantes coloridos, conforme a imagem anexada:

 - Diamante vermelho: Indica que nenhum teste está cobrindo o branch;
   
 - Diamante amarelo: Indica que o código está parcialmente coberto;
   
 - Diamante verde: Indica que todo o branch foi testado e coberto;

  ![image](https://github.com/Sammy192/DSMovie_springExpert/assets/53224915/b3c725a1-77a3-419e-9f3b-7d4e2d9ae9ad)
![image](https://github.com/Sammy192/DSMovie_springExpert/assets/53224915/fd146de2-70d9-44f1-869b-5c36049a8f9f)

