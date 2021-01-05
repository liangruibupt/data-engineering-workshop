# Lab 4: Data Lake Automation with Lake Formation

This lab will give you an understanding of the AWS Lake Formation – a service that makes it easy to set up a secure data lake in days

![lakeformation-arch](media/lakeformation-arch.png)

The [DMS Lab](Ingestion-with-DMS.md) and [Glue ETL lab](Transforming-data-with-Glue.md) is a prerequisite for this lab.

Tasks Completed in this Lab:
1. Create a JDBC connection to RDS in AWS Glue
2. Lake Formation IAM Role
3. Lake Formation – Add Administrator and start workflows using Blueprints
4. Explore the components of a Glue WorkFlow created by lake formation
5. Explore workflow results in Athena

## Data-Lake-Automation-with-LakeFormation
- [Setup Network Configuration](https://aws-dataengineering-day.workshop.aws/1200/sagemaker.html#setup-network-configuration)
- [Create an IAM role to use with Lake Formation](https://aws-dataengineering-day.workshop.aws/1200/sagemaker.html#create-an-iam-role-to-use-with-lake-formation)
- [Create Glue JDBC connection for RDS](https://aws-dataengineering-day.workshop.aws/1200/sagemaker.html#create-glue-jdbc-connection-for-rds)
- [Lake Formation start workflows using Blueprints](https://aws-dataengineering-day.workshop.aws/1200/sagemaker.html#lake-formation--add-administrator-and-start-workflows-using-blueprints)
- [Explore the Underlying Components of a Blueprint](https://aws-dataengineering-day.workshop.aws/1200/sagemaker.html#explore-the-underlying-components-of-a-blueprint)
- [Explore workflow results in Athena](https://aws-dataengineering-day.workshop.aws/1200/sagemaker.html#explore-workflow-results-in-athena)