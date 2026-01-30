Developed and deployed a personal resume website using AWS S3 for static hosting.Leveraged cloud storage and 
scalable infrastructure to ensure high availability and low latency. –Utilized AWS Services: S3, Route 53, CloudFront, IAM for hosting, DNS, CDN, and access management. Built the 
frontend using HTML5, CSS3, and JavaScript for a responsive design.Implemented automation and version control using 
AWS CLI and Git. 

How the Website Is Deployed Using AWS

1️⃣ Amazon S3 – Website Hosting

What it does:

Stores and serves your resume website files.

How it’s used:

Create an S3 bucket.

Upload website files (index.html, CSS, JS).

Enable Static Website Hosting.

Allow public read access using a bucket policy.

Result:Your resume becomes accessible using an S3 website URL.

2️⃣ AWS IAM – Access Management

What it does:

Controls who can access AWS resources.

How it’s used:

Create an IAM user.

Give permissions to manage S3 and CloudFront.

Generate access keys.

Use these keys with AWS CLI to upload and update files securely.

Result:Only authorized users can deploy or modify the website.

3️⃣ Amazon CloudFront – CDN (Fast Delivery)

What it does:

Makes the website load faster globally.

How it’s used:

Create a CloudFront distribution.

Set the S3 bucket as the origin.

Enable caching and HTTPS.

Set index.html as default page.

Result:Users access the website from the nearest CloudFront edge location.
4️⃣ Amazon Route 53 – DNS (Custom Domain)

What it does:

Connects your domain name to the website.

How it’s used:

Create a hosted zone for your domain

Create a DNS record.

Point the domain to the CloudFront distribution.

Result:Your resume opens using a custom domain name.
