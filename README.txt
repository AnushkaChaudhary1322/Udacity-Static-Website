# Deploy Static Website on AWS

## Project Overview

This project demonstrates the deployment of a **static website on Amazon Web Services (AWS)** using **Amazon S3** and **Amazon CloudFront**. The goal of this project is to host a static website with high availability, global content delivery.

The website files are uploaded to an S3 bucket, configured for static website hosting, and distributed globally using CloudFront.

---

## Project Files

The following files and folders are included in this project:

* **index.html** – The Index document for the website.
* **/img** – The background image file for the website.
* **/vendor** – Bootssrap CSS framework, Font, and JavaScript libraries needed for the website to function.
* **/css** – CSS files for the website.
* **/screenshots** – Contains screenshots of AWS configurations and deployed website.

---

## AWS S3 Configuration

* An **S3 bucket** is created to host the static website.
* All website files are **successfully uploaded** to the S3 bucket.
* The S3 bucket is **configured for static website hosting**.
* The **"Block all public access"** setting is turned **off**.
* A **bucket policy** is applied using IAM to make the website contents **publicly accessible**.

---

## IAM Roles & Policies

* IAM is used to manage access permissions securely.
* A **bucket policy** is attached to the S3 bucket to allow public read access (`GetObject`).
* IAM ensures controlled and secure access to AWS resources.

---

## CloudFront Distribution

* **Amazon CloudFront** is configured as a Content Delivery Network (CDN).
* CloudFront retrieves website files from the S3 bucket (origin).
* The distribution improves performance by serving content from edge locations.
* HTTPS support is enabled through CloudFront for secure access.

---

## Website Access

* The website is accessible directly using the **S3 static website endpoint**.
* The website is also accessible using the **CloudFront distribution URL**.
* The CloudFront URL works across **multiple devices and browsers**, ensuring consistent global access.

---

## Deployed URLs

* **S3 Website URL:**

  ```
  http://my-754408559350-bucket.s3-website-us-east-1.amazonaws.com/
  ```

* **CloudFront URL:**

  ```
  https://dozcf2h5wo5h4.cloudfront.net/index.html
  ```

---

## Screenshots

All screenshots are stored inside the `screenshots/` folder. The images will be visible directly on GitHub using the paths below.

### S3 Bucket Creation

![S3 Bucket Created](screenshots/s3-bucket-created.png)

### Files Uploaded to S3 Bucket

![Files Uploaded to S3](screenshots/s3-files-uploaded.png)

### Static Website Hosting Enabled

![Static Website Hosting](screenshots/s3-static-website-hosting.png)

### Public Access Settings & Bucket Policy

![S3 Bucket Policy](screenshots/s3-bucket-policy.png)

### CloudFront Distribution Configuration

![CloudFront Distribution](screenshots/cloudfront-distribution.png)

### Website Access via S3 URL

![Website via S3](screenshots/website-s3-url.png)

### Website Access via CloudFront URL

![Website via CloudFront](screenshots/website-cloudfront-url.png)

### CloudFront URL on Different Devices

![CloudFront Multiple Devices](screenshots/cloudfront-multiple-devices.png)

---

## 📁 Folder Structure

```
UDACITY-STARTER-WEBSITE/
│── index.html
│── README.txt
│── css/
│── img/
│── vendor/
│── screenshots/

```

---

## Project Outcome

* Static website successfully hosted on Amazon S3
* Public access enabled using IAM bucket policy
* Global content delivery achieved using CloudFront
* Website accessible via both S3 and CloudFront URLs

---

## Conclusion

This project demonstrates a complete static website deployment on AWS using industry best practices. By leveraging S3 for storage, CloudFront for content delivery, and IAM for access control.

