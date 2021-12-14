node {
    stage('Build') {
          withMaven(maven: 'maven3_5_2') {
              sh "mvn clean install"
              withSonarQubeEnv('MySonarqubeServer') {
               sh "mvn sonar:sonar"
        }
          }
              
          }
}
