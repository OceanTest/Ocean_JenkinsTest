node('slave1'){
    // Mark the code checkout 'stage'....
    stage('Checkout'){
    // Get some code from a GitHub repository
    git([url: 'https://github.com/OceanTest/Ocean_JenkinsTest.git', branch: 'master'])
    // Mark the code build 'stage'....
    }  
    // Mark the code run 'stage'....
    stage('Run'){
    // Run the program
    sh script:"ssh root@10.25.132.123 'cd /home/workspace;python3 ocean.py'"
    }
}