node {
    // Clean workspace before doing anything
    deleteDir()

    try {
        stage ('Job 1') {
           echo "Job 1"
        }
        stage ('Job 2') {
             echo "'Job 2'"
        }
       
        stage ('Job 3') {
            echo "Job 3"
        }
    } catch (err) {
        currentBuild.result = 'FAILED'
        throw err
    }
}
