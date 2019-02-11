# performance
Running performance tests  with JMeter and Taurus 
Usage

Make sure this repository has a webhook set up for the Jenkins server you're using.

Make sure your Jenkins server has the Performance Plugin installed.

Create a new  Pipeline project in Jenkins and point it to this github repository.

Assign the PerformanceJenkinsFile in this directory as the JenkinsFile for the new project

By default the project will run tests on the ANG dev instance with a thread and iteration count of 1. To change this, run the test with parameters. You will be able to choose which environment it runs on, set certain testing parameters, and choose whether to run it with Taurus or just as a plan JMeter test. Running with Taurus will give you an easier to digest output, while running as plain JMeter will provide you the raw output file in the build artifacts, which you can use to get more detailed testing result.
