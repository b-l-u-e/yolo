
 # Ansible Playbooks
 We run the conteinerized app through playbooks 
 ### Steps
 1. Create required files
     * ansible.cfg -this states our inventory location
     * Vagrantfile 
     * hosts -this is our inventory that has the defined servers
     * playbook.yml - this has our main play
     * vars.yml - we define our variables in this file and import them into playbook.yml
 2. Initialize roles for abstraction purposes
     ```
     ansible-galaxy init <roleName>
     ```
     We will use 3 roles in this case and add them to a role folder
     1. git - Installs git
     1. docker -Installs dependencies, docker and docker-compose
     1. docker-compose -Starts our docker compose
    
 3. Run the playbook through vagrant provision
      ```
      vagrant up
      ```
    This autmatically provisions as stated in the Vagrantfile.
   
      ```
      vagrant provision
      ```
 4. After the play runs to completion, yoou can access the app through the browser
      [http://localhost:3000](http://localhost:3000)
      This is made possible by the forwarded ports added in Vagrantfile
      ```
      config.vm.network "forwarded_port", guest: 3000, host: 3000, protocol: "tcp"
      config.vm.network "forwarded_port", guest: 5000, host: 5000, protocol: "tcp"
  
      ```
 5. Add products to the app and confirm data persistence

 # Kubernetes

 Kubernetes Essentials

 Here are the some docs to understand concepts of kubernetes

 - [Kubernetes Docs](https://kubernetes.io/docs/concepts/)

 - [How to get started with Kubernetes](https://medium.com/bb-tutorials-and-thoughts/how-to-get-started-with-kubernetes-e06ea82d23b)

 ### GCP Prerequisties

 - Step 1: Create a New Project

 - Step 2: Need to create a Billing Account

 - Step 3: Link billing account with the project created on step 1

 - Step 4: Enable APIs that will need to run the dataflow on GCP

 - Step 5: Download the Google SDK


### Install gcloud CLI and Configure

Once GCP account is create can install gcloud CLI tool.

The gcloud CLI is part of the [Google Cloud SDK](https://cloud.google.com/sdk/docs). Must [download and install the SDK](https://cloud.google.com/sdk/docs/install) on your system and [initialize it](https://cloud.google.com/sdk/docs/initializing) before using gcloudCLI tool