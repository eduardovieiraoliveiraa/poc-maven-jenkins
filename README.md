Projeto criado via terminal para testar build com jenkins 

SO: Ubuntu
Programas instalados: vim, git, maven, java 17, jeunkins 


Apos instalar o java eexcute:
export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
export PATH=$JAVA_HOME/bin:$PATH
source ~/.bashrc


Após install o jenkins em tools você deve adc o plugin maven e java passando o JAVA_HOME

passo a passo:

comando executado: mvn archetype:generate -DgroupId=com.exemplo -DartifactId=teste-jenkins -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

cd /home/seu projeto
git init
git add . 
git commit -m "commit inicial"
git remote add origin "sua url"
git push -u origin master

irá pedir usuario e senha do git, a senha agora é necessário gerar um token em settings/developer settings/personal access tokens (tekens classic) e gere o token de acesso

crie um job no jenkins, como freestyle project,em build steps configure como maven targets
em goals coloque o comando desejado
