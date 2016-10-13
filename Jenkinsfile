node {
  git url: 'https://github.com/nandotorres/azure-deploy-tomcat-teste.git'
  def mvnHome = tool 'M3'
  env.PATH = "${mvnHome}/bin:${env.PATH}"
  sh "${mvnHome}/bin/mvn -B -Dmaven.test.failure.ignore clean install"
  step([$class: 'ArtifactArchiver', artifacts: '**/target/*.jar', fingerprint: true])
}

