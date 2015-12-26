**ANSIBLE FOR IDK**

This is a basic setup for deployment to a server on EC2.
Currently it installs system dependencies, creates a virtualenv and installs python dependencies.
Run with: ansible-playbook playbook.yml --extra-vars "repo_tag commit_hash"


    TODO:

    Setup codeship deploy to S3 and a webhook to a server.
    
    Retrieve artifact from S3.

    Install application.

    Copy the local .env to server to finish the application setup.

    Install nginx and uwsgi. Still need to define which is the best way to setup the     configuration files for those, but for now will copy them from the repository or a file generated from a vault.
    
