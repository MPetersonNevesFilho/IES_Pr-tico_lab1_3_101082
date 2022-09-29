Primeiramente, foi utilizado a linha abaixo para gerar este ficheiro:
mvn archetype:generate -DgroupId=ex2 -DartifactId=lab1_2 -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

Depois, alterou-se no pom>properties>maven.compiler.source&&target>>agora:17-antes:1.7

Porém, devido a inexperiência, o projeto não foi criado como deveria, sendo necessário excluir a primeira versão e criar uma nova. Para tal, foi utilizado o passo a passo da IDE VS Code. Nesse momento, foi criado o projeto com o nome de lab1_2, neste, foi alterado o POM com informações sobre o desenvolvedor em questão e alterado o valor do compilador Maven.

Depois da adatação do código foi utilizado tais linhas:
mvn package
mvn exec:java -D"exec.mainClass=ex2.App"