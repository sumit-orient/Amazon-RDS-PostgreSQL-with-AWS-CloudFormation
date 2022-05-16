# Amazon RDS PostgreSQL with AWS CloudFormation


## 1. Launch AWS CloudShell

1. Sign in to AWS Management Console <img src="https://github.com/t2yijaeho/Amazon-RDS-PostgreSQL-with-AWS-CloudFormation/blob/matia/images/AWS%20Management%20Console.png?raw=true" width="16">

2. Choose the AWS CloudShell icon <img src="https://github.com/t2yijaeho/Amazon-RDS-PostgreSQL-with-AWS-CloudFormation/blob/matia/images/AWS%20CloudShell.png?raw=true" width="16"> on the navigation bar

3. Check AWS Command Line Interface (AWS CLI) version

    ```bash
    aws --version
    ```

    <img src="https://github.com/t2yijaeho/Amazon-RDS-PostgreSQL-with-AWS-CloudFormation/blob/matia/images/AWS%20CloudShell%20version.png?raw=true">


## 2. Create an Amazon RDS PostgreSQL

1. Get an AWS CloudFormation stack template body

    ```bash
    wget https://raw.githubusercontent.com/t2yijaeho/Amazon-RDS-PostgreSQL-with-AWS-CloudFormation/2eb837192a05043afdb3148586fc8e90a3baa8ad/Template/RDS-PostgreSQL.yaml
    ```


2. Create an AWS CloudFormation stack

    ```bash
    aws cloudformation create-stack \
      --stack-name RDS-PostgreSQL \
      --template-body file://./RDS-PostgreSQL.yaml
    ```

3. AWS CloudFormation returns following output

    ```json
    {
    "StackId": "arn:aws:cloudformation:us-abcd-x:123456889012:stack/RDS-PostgreSQL/b4d0f5e0-d4c2-11ec-9529-06edcc65f112"
    }
    ```

4. Monitor the progress by the stack's events in AWS management console

    <img src="https://github.com/t2yijaeho/Amazon-RDS-PostgreSQL-with-AWS-CloudFormation/blob/matia/images/CloudFormation%20Stack%20Creation%20Events.png?raw=true">

