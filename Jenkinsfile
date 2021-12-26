// pipeline {
//     agent any
//
//     stages {
//         stage('One') {
//             steps {
//                 echo 'Hi World'
//             }
//         }
//         stage('Two') {
//             steps {
//                 echo 'Hi World'
//             }
//         }
//         stage('Three') {
//             steps {
//                 echo 'Hi World'
//                 echo 'Hello from Stage Three'
//             }
//         }
//     }
// }
// -------------------------------------------
// pipeline {
//     agent { label 'WORKSTATION' }
//      options {
//             ansiColor('xterm')
//         }
//     stages {
//         stage('Ansible Playbook run') {
//             steps {
//              sh 'ansible-playbook 01-simple-playbook.yml'
//             }
//         }
//     }
// }
// -----------------------------------------------------
// pipeline {
//     agent { label 'WORKSTATION' }
//      options {
//             ansiColor('xterm')
//         }
//
//     stages  {
//         stage('Ansible Playbook run') {
//             steps {
//                 sh 'ansible-playbook 01-simple-playbook.yml'
//             }
//         }
//     }
// }
// ---------------------------------
// pipeline {
//     agent any
//
//     stages {
//         stage('stage1') {
//             steps {
//                 sh 'echo -e "\\e[1;32mThis code is from git\\e[0m"'
//                 sh 'echo -e "\\e[1;33mfor Pipeline Declarative script\\e[0m"'
//             }
//         }
//     }
// }
// ----------------------------------------
// Agent syntax example
// pipeline {
//     agent any
//     agent none
//     agent {
//         node { 'node1'}
//     }
//     agent { label 'ANSIBLE' && 'CENTOS'}
//   }
//   stages {
//     stage('sample') {
//         agent { label 'UBUNTU'}
//         steps {
//          sh 'echo hello'
//         }
//     }
//   }
// ------------------------------------------
// options example
// pipeline {
//     agent any
//     options {
//         disableConcurrentBuilds()
//     }
//
//     stages  {
//         stage('options example') {
//             steps {
//                 sh 'sleep 10'
//             }
//         }
//     }
// }
// -------------------------------------------
// environment example
// pipeline {
//     agent any
//     environment {
//         URL1 = 'google.com'
//     }
//     stages {
//         stage('ENV example') {
//             steps {
//                 sh 'echo ${URL1}'
//                 echo URL1
//             }
//         }
//     }
// }
// ------------------------------------------------
// reading secrets using environment variable

pipeline {
    agent any
    environment {
        SSH = credentials('CENTOS')
        SSH1 = credentials("common/ssh")
    }
    stages {
        stage('reading secrets') {
            steps {
                echo SSH
                sh 'env'
                echo SSH1
                sh 'echo ${SSH1} | base64'

            }
        }
    }

}





































