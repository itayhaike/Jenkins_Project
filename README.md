# Jenkins_Project
1) You need to save all your source code in GitHub including Jenkinsfile of your pipeline.
Your pipeline should be triggered after each commit. (Build per checkin)
You need to create choice parameter "Language" with the values: All, C, Python, Bash.
When the pipeline is triggered automatically "All" value has to be choosen.
Each stage of the pipeline is running particular script on a language.
When you choose a particular language the pipeliline has to execute only stages regarding the language.
If you choose python the pipeline will execute only stages of python
If you choose bash the pipeline will execute only stages of bash.
All other scripts execution has to be skipped in this cases.
The pipeline should include minimum 3-4 stages. More will be appreciated.
To add log files algorithm like on file Jenkinsfile_adv.

To create an image of your VM and to notify which pipeline name to run 
