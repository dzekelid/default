---
name: AWS ElastiCache
x-slug: aws-elasticache
description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
  and scale an in-memory data store or cache in the cloud. The service improves the
  performance of web applications by allowing you to retrieve information from fast,
  managed, in-memory data stores, instead of relying entirely on slower disk-based
  databases. Amazon ElastiCache automatically detects and replaces failed nodes, reducing
  the overhead associated with self-managed infrastructures and provides a resilient
  system that mitigates the risk of overloaded databases, which slow website and application
  load times. Through integration with Amazon CloudWatch, Amazon ElastiCache provides
  enhanced visibility into key performance metrics associated with your Redis or Memcached
  nodes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Default
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/aws-elasticache/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon ElastiCache API Describe Engine Default Parameters
  x-api-slug: amazon-elasticache-api
  description: |-
    Returns the default engine and
                system parameter information for the specified cache engine.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DescribeEngineDefaultParameters
  tags: Engine Default Parameters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/aws-elasticache/actiondescribeenginedefaultparameters-get-openapi.md
- name: Amazon ElastiCache API
  x-api-slug: amazon-elasticache-api
  description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
    and scale an in-memory data store or cache in the cloud. The service improves
    the performance of web applications by allowing you to retrieve information from
    fast, managed, in-memory data stores, instead of relying entirely on slower disk-based
    databases. Amazon ElastiCache automatically detects and replaces failed nodes,
    reducing the overhead associated with self-managed infrastructures and provides
    a resilient system that mitigates the risk of overloaded databases, which slow
    website and application load times. Through integration with Amazon CloudWatch,
    Amazon ElastiCache provides enhanced visibility into key performance metrics associated
    with your Redis or Memcached nodes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/aws-elasticache/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonElastiCache/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/elasticache/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticache/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticache/pricing/
- type: x-resources
  url: https://aws.amazon.com/elasticache/developer-resources/
- type: x-testimonials
  url: https://aws.amazon.com/elasticache/testimonials/
- type: x-website
  url: https://aws.amazon.com/elasticache/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---