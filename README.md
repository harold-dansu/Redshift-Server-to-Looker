# Redshift-Server-to-Looker

IN AWS
- Edit your Redshift Serverless workgroup settings to be publicly available. This will allow instances outside your VPC to connect to your database through the cluster endpoint.
- Copy the JDBC URL
- Last navigate to https://s3.amazonaws.com/redshift-downloads/redshift-ssl-ca-cert.pem. This will automatically download the certificate you need in Looker. 

IN LOOKER
- Select the Redshift connector option
- Paste your JDBC URL
- Enter your Redshift Serverless database username and password
- Upload the Amazon Redshift SSL certificate

You should be able to see your tables thereafter
