node {

    stage("Checkout") {
        checkout scm
    }

    stage("Run") {
        sh "python app.py"
    }
}
