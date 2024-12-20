pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // 使用拉取的 Node.js 镜像
                    docker.image('node:14').inside {
                        sh 'npm install'
                    }
                }
            }
        }
        // 其他阶段...
    }
}