node {
  git url: 'https://github.com/nandotorres/azure-deploy-tomcat-teste.git'
  def mvnHome = tool 'M3'
  env.PATH = "${mvnHome}/bin:${env.PATH}"
  sh 'mvn -B verify'   
}