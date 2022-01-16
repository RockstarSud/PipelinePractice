node {
  stage('Checking maven version') {
    sh 'mvn -v'
  }
  stage('Cloning Git repository') {
    git credentialsId: '7a62acaa-13b9-4aa6-8a90-32d34c1b1371', url: 'https://github.com/RockstarSud/Cucumber4-With-POM.git'
  }
  stage('Deploy') {
    sh 'mvn clean test'    
  }
}
