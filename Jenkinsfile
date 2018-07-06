node(ocean_windows_testnode){
    // Mark the code checkout 'stage'....
    stage('Checkout'){
    // Get some code from a GitHub repository
    git([url: 'https://github.com/OceanTest/Ocean_JenkinsTest.git', branch: 'master'])
    // Mark the code build 'stage'....
    }  
    // Mark the code run 'stage'....
    stage('Run'){
    // Run the program
    sh 'python test.py'
    }
}