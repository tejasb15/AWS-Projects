# Static Web Hosting using Amazon S3 and CloudFront 🌐

## **Overview**
This project demonstrates how to host a static website using **Amazon S3** and enhance its performance with **CloudFront**, AWS's Content Delivery Network (CDN). The goal is to provide a scalable, durable, and globally distributed solution for hosting static web content, like HTML, CSS, and JavaScript.

---

## **Architecture Diagram**
Below is the architecture of the static web hosting solution using Amazon S3 and CloudFront:

![S3 and CloudFront Architecture](images/s3-cloudfront-architecture.png)

!
---

## **Key Features**
- **S3 Static Website Hosting**: 
  - Store and host static web content with high durability and availability.
  - Cost-effective and easy-to-manage web hosting solution.
- **CloudFront Integration**: 
  - Enhanced global content delivery with reduced latency.
  - Secure and scalable distribution using AWS's global infrastructure.

---

## **Objectives**
1. Deploy a static website with a public S3 bucket.
2. Use **CloudFront** to distribute content with low latency.
3. Enable SSL/TLS for secure content delivery.
4. Demonstrate cost-effective and scalable static hosting.

---

## **Steps to Host the Website**
### **1. Amazon S3 Setup**
- Create an S3 bucket for hosting the static content.
- Enable public access and add a bucket policy for public-read access.
- Upload the static files (e.g., `index.html`) to the S3 bucket.

### **2. Enable Static Website Hosting**
- Configure the bucket to serve as a static website.
- Specify the index document (e.g., `index.html`) and optional error document.

### **3. Integrate CloudFront**
- Create a CloudFront distribution for the S3 bucket.
- Configure the origin domain and enable public access.
- Use the CloudFront domain name to access the hosted website.

---

## **Architecture**
- **Amazon S3**: Object storage for static content with public-read access.
- **Amazon CloudFront**: CDN for global delivery, caching, and performance improvement.
- **Website Endpoint**: Direct access through S3 and CloudFront domain.

---

## **Limitations**
- **No server-side processing**: Suitable only for static content.
- **Security configurations**: Requires careful bucket policies to avoid unauthorized access.
- **Custom error pages**: Limited compared to traditional web servers.

---

## **Advantages**
- **High Availability**: 99.999999999% (11 nines) durability.
- **Scalability**: Automatically handles increased traffic.
- **Low Latency**: Content cached closer to users through edge locations.
- **Cost-Effective**: Pay-as-you-go pricing.

***

## **Testing the Website**
- Access the website using the S3 endpoint.
- Test the CloudFront distribution domain for faster and secure content delivery.

***

## **Future Enhancements**
- Add **AWS Lambda@Edge** for dynamic content.
- Use **AWS Route 53** for custom domain integration.

---

## **Author**
**Tejas Bharambe**  
Full Stack Developer | AWS Enthusiast  
[GitHub](https://github.com/tejasb15) | [LinkedIn](https://linkedin.com/in/tejas-bharambe)

---

## **References**
- [Amazon S3 Documentation](https://docs.aws.amazon.com/s3/)
- [Amazon CloudFront Documentation](https://docs.aws.amazon.com/cloudfront/)

---

