pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings', description: 'How should I greet the world?')
        string(name: 'FirstOption', value: "test")
        string(name: 'AnotherOption', value: "test12")
        
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Hello} World!"
            }
        }
    }
}
