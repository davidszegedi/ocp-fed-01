# ocp-cluster-01

1 - Git clone this repository on you local folder (your user should have sudo privileges)

2 - Create AWS credentials in your home folder:

        $ cat ~/.aws/credentials

        ; https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
        [default]
        aws_access_key_id     = ***********
        aws_secret_access_key = ***********

3 - Create a var file to define the vars below:

    $ cat secret.json

    { "var_pullsecret": *****, "var_sshkey": *****, "var_pullsecretjson": *****}

   To prepare your environnement, launch "01-Prepare-environment.yml" playbook with these extra vars passed

4 - To deploy the three OCP 4 clusters, launch "02-Deploy-cluster.yml" playbook

5 - To deploy the federated environment, launch "09-Deploy-demo.yml" playbook

...

6 - To clean deployment, launch "10-Destroy-cluster.yml" playbook
