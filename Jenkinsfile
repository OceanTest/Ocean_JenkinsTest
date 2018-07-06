def testnode1 = env.testnode1
def testnode2 = env.testnode2
def Nodelist = [testnode1, testnode2]

node('slave1'){
    // Mark the code checkout 'stage'....
    stage('Checkout'){
        // Get some code from a GitHub repository
        git([url: 'https://github.com/OceanTest/Ocean_JenkinsTest.git', branch: 'master'])
        
    }
    // Mark the code GetParameter 'stage'....
    stage('GetParameter'){
    // Run the program
        Nodelist.each{Node -> println "\r\n Test node is " Node}
    }
    // Mark the code Run 'stage'....
    stage('Run'){
        // Run the program
        sh script:"ssh root@10.25.132.123 'cd /home/workspace;python3 ocean.py'"
    }
}
