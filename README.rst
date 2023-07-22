AWS Resources Report Generator

This script generates a comprehensive report of various AWS resources, including EC2 instances, S3 buckets, AMIs, and snapshots. The report is generated in the form of an Excel file and can be emailed to the desired recipients using the Simple Email Service (SES).
Prerequisites

Before running the script, ensure that you have the following prerequisites:

    AWS Credentials: Obtain valid AWS access key ID and secret access key with sufficient permissions to access EC2, S3, and SES.

Usage

    Clone this repository to your local machine.

    Update the following variables in the code:

        access_key_id and secret_access_key: Provide your AWS access key ID and secret access key.

        SENDER and RECIPIENT: Specify the sender and recipient email addresses for sending the report.

        BUCKET_NAME and KEY: Provide the name of the S3 bucket where you want to upload the report and the desired object key.

    Run the script using Python: python script.py.

    The script will gather information about running EC2 instances, S3 buckets, AMIs, and snapshots. It will generate an Excel report named AWSresourcesReport.xlsx in the /tmp/ directory.

    The report will contain multiple sheets, each presenting information about a specific AWS resource.

    The report will also include visualizations such as a bar chart depicting the time consumption of EC2 instances.

    The generated report will be uploaded to the specified S3 bucket.

    An email containing the report will be sent using SES to the specified recipient.

Additional Considerations

    Ensure that you have the necessary IAM permissions to access and manage the desired AWS resources.

    Customize the script as per your requirements, such as adding more AWS resources or modifying the report format.

    Schedule the script to run periodically using AWS Lambda or any other desired method to automate the report generation process.

Please note that this README provides a high-level overview of the script's functionality. For detailed usage and configuration instructions, refer to the comments in the code and the official documentation for AWS services and Python libraries used.

Feel free to reach out if you have any questions or need further assistance.
