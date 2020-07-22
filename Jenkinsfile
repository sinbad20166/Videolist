pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings', description: 'How should I greet the world?')
        choice(name: 'HelloChoice', defaultValue: 'A', 'B', description: 'Choices Given?')
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Hello} World!"
                echo "${params.HelloChoice}"
            }
        }
    }
}
