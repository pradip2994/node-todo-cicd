```
sudo apt install nodejs
sudo apt install npm
npm install
node app.js
```
# Automated CICD Pipeline for Node Js web application using AWS, Github Integration and webhook, Docker,Docker-compose and Jenkins.

Generate the SSH keys for integrating  Jenkins project with your git repository. Use ssh-keygen command to create public and private keys in EC2.
1) Configuring GitHub
  Go to your GitHub account settings.
  Go to “SSH and GPG” keys, Add the public key that we created using ssh-keygen for Authentication.
2)  For Installing GitHub Integration plugin in Jenkins
  1.In jenkins dashboard.
  2.Click on the “Manage Jenkins” button 
  3.Click on “Manage Plugins”
  4. Install “GitHub Integration” plugin
3) For GitHub-Webhook:
  1.Go to your GitHub repository and click on Settings.
  2.Click on Webhooks and then click on Add webhook.
  3. In the ‘Payload URL’ field, paste your Jenkins environment URL. At the end of this URL add /github-webhook/. In the ‘Content type’ select: ‘application/json’ and leave the ‘Secret’ field empty.
4) Configuring Jenkins:
  1. Create a jenkins job
  2. Create node-todo-app freestyle project
  3. In Configure, GitHub project URL paste project GitHub URL
  4.In Git, add credentials for jenkins
  5. Add the private key which we created using the ssh-keygen command in EC2.
  6. Click on the ‘Build Triggers’ tab and tick on the ‘GitHub hook trigger for GITScm polling’.
  7. Then save it.
  8.  Make the changes to the existing file in github repo or  Create the new file.
  9. See Output.

![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/7ad72692-b93d-4c02-b83a-053fc0d2fa2f)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/06ee70db-2fdb-41ad-84e3-2b53c4a3d25e)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/954cc886-5199-4f28-98be-3eb6242a5aa2)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/6d83d36e-0ed4-4242-a236-4331f2758caa)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/84ddcd7e-7fc5-47e0-8e1f-5a93c4040d52)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/6a5d7f5b-d153-459f-8416-5fb5c6d7e6d8)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/06665804-5c2d-406e-beb4-5aea2dbc7e80)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/c6d76680-da93-4dd6-964a-e0bf545d5dc7)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/8a24a387-fa11-4533-a6d0-8576347e52c9)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/de1b1e4b-d8ef-47b8-a72f-c90fec9a5469)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/a77e6e14-299b-44f6-8528-f4a670a89c98)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/3a8cb2f6-5851-4eb7-a85d-98983dbe2ccb)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/01f006e5-249c-4b77-89d7-28034c790489)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/da389f0e-3bae-48fd-87ee-5d132e92ba5e)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/03d413d9-15bc-41d0-a744-4c13d8d8c7ad)
![image](https://github.com/pradip2994/jenkins-CICD-main/assets/124191442/9c4cb53f-f729-4959-8832-e550d4346571)
