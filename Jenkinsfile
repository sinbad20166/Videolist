pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings', description: 'How should I greet the world?')
        string(name: 'FirstOption', defaultValue: 'test', description: 'First Option')
        string(name: 'AnotherOption', defaultValue: 'test12', description: '2nd Option')
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Hello} World!"
                echo "${params.FirstOption} 1st!"
                echo "${params.AnotherOption} 2nd!"
            }
        }
    }
}
