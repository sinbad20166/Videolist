pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings', description: 'How should I greet the world?')
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Greeting} World!"
            }
        }
    }
}
