Projeto criado via terminal para testar build com jenkins 

SO: Ubuntu
Programas instalados: vim, git, maven, java 17, jeunkins 

passo a passo:

comando executado: mvn archetype:generate -DgroupId=com.exemplo -DartifactId=teste-jenkins -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

cd /home/seu projeto
git init
git add . 
git commit -m "commit inicial"
git remote add origin "sua url"
git push -u origin master

irá pedir usuario e senha do git, a senha agora é necessário gerar um token em settings/developer settings/personal access tokens (tekens classic) e gere o token de acesso
