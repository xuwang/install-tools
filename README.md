# Instructions for tools installation on MacOS. 

Install common DevOps tools - terraform, jq, vagrant, awscli, etc.

**Install AWS CLI and Setup AWS credentials**

Go to [AWS Console](https://console.aws.amazon.com/).

* Signup AWS account if you don't already have one. 
* Create a group `group` with `aws-policy` policy.
* Create an IAM user `user` and __Download__ the user credentials.
* Add user `user` to group `group`.
* Install [AWS CLI](https://github.com/aws/aws-cli)

    ```
    $ brew install awscli
    ```
    or

    ```
    $ sudo easy_install pip
    $ sudo pip install --upgrade awscli
    ```

* Setup AWS credential file

  Use aws command to create credential file. The values you  provide  for the AWS Access Key ID and the AWS
  Secret Access Key will  be  written  to  the  shared  credentials file (~/.aws/credentials).

```
$ aws configure [--profile profile-name]
```

**Install [Terraform](http://www.terraform.io/downloads.html)**
```
$ brew update
$ brew install terraform
```
or
```
$ mkdir -p ~/bin/terraform
$ cd ~/bin/terraform
$ curl -L -O https://releases.hashicorp.com/terraform/0.6.12/terraform_0.6.12_darwin_amd64.zip
$ unzip terraform_0.6.12_darwin_amd64.zip
```

**Install [Jq](http://stedolan.github.io/jq/)**

```
$ brew install jq
```

**Install Vagrant**

See [Vagrant](https://www.vagrantup.com/)
