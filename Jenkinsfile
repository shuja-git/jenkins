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
//     agent any
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
//                 sh 'echo -e "\\e[1;32mGreenColor\\e[0m"'
//                 sh 'echo -e "\\e[1;33mYelloColor\\e[0m"'
//             }
//         }
//     }
// }















