elifeLibrary {
    stage 'Checkout', {
        checkout scm
    }

    stage 'Build image', {
        sh 'docker build -t elife/sciencebeam-gym .'
    }

    stage 'Run tests', {
        elifeLocalTests './project_tests.sh'
    }
}
