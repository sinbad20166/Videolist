pipeline {
    agent { label 'master' }
    build job:'NameOfTheJob', parameters: [
      string(name: 'FirstOption', value: "test"),
      string(name: 'AnotherOption', value: "test12")
]
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings', description: 'How should I greet the world?')
        
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Hello} World!"
            }
        }
    }
}
