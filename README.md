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
