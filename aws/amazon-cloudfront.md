# Key review: Amazon CloudFront

<b>Amazon CloudFront</b> is a fast, secure, and programmable content delivery network (CDN) offered by Amazon Web Services (AWS). It provides a global network of servers, called edge locations, to cache and deliver content from AWS services and other origin servers to users all over the world.

## Purposes

- Amazon CloudFront can accelerate the delivery of static, dynamic, and streaming content to users around the world.
- Amazon CloudFront can help reduce latency, improve reliability, and lower data transfer costs for your website or application.
- Amazon CloudFront can provide security and protection against malicious attacks such as distributed denial-of-service (DDoS) attacks.

## Features

### Content delivery
- Amazon CloudFront can deliver content from AWS services such as Amazon S3, Amazon EC2, and Amazon Elastic Load Balancing (ELB).
- Amazon CloudFront can also deliver content from other origin servers such as HTTP servers and media servers.
- Amazon CloudFront supports both static and dynamic content, including HTML, CSS, JavaScript, images, videos, and live and on-demand streaming media.
- Global network
- Amazon CloudFront has a global network of edge locations in more than 200 cities around the world.
- Edge locations are geographically distributed to reduce latency and improve performance for users in different regions.
- Edge locations can cache content and serve it directly to users, reducing the load on origin servers and improving performance.

### Security
- Amazon CloudFront can provide security and protection against malicious attacks such as DDoS attacks.
- Amazon CloudFront can also encrypt content in transit using SSL/TLS certificates.
- Amazon CloudFront can integrate with AWS Shield, a managed DDoS protection service, to provide additional security against DDoS attacks.

### Programmability
- Amazon CloudFront is programmable using APIs and can be integrated with other AWS services and third-party services.
- Amazon CloudFront supports custom headers, cookies, and query string parameters for caching and content delivery.
- Amazon CloudFront supports Lambda@Edge, a serverless computing service that allows you to run custom code at the edge locations.

## Advantages

- <b>High performance</b>: Amazon CloudFront can improve the performance and speed of content delivery by caching content at edge locations and reducing latency.
- <b>Scalability</b>: Amazon CloudFront can handle high volumes of traffic and can scale automatically based on demand.
- <b>Security</b>: Amazon CloudFront provides security and protection against malicious attacks such as DDoS attacks.
- <b>Programmability</b>: Amazon CloudFront is programmable and can be integrated with other AWS services and third-party services.

## Disadvantages

- <b>Cost</b>: Amazon CloudFront can be more expensive than other AWS services, especially if you have high data transfer or request rates.
- <b>Complexity</b>: Amazon CloudFront can be complex to configure and manage, especially if you need to use custom headers, cookies, or query string parameters.
- <b>Caching</b>: Amazon CloudFront's caching behavior can be unpredictable, especially if you have dynamic content or frequently changing content.

Overall, Amazon CloudFront is a powerful and flexible CDN that can accelerate the delivery of content and improve the performance and reliability of your website or application. However, it's important to carefully consider the cost and complexity of using Amazon CloudFront and to design your content delivery strategy accordingly.

[aws-documentation](https://docs.aws.amazon.com/cloudfront/?icmpid=docs_homepage_networking)