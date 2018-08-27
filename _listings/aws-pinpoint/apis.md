---
name: AWS Pinpoint
x-slug: aws-pinpoint
description: Amazon Pinpoint makes it easy to run targeted campaigns to drive user
  engagement in mobile apps. Amazon Pinpoint helps you understand user behavior, define
  which users to target, determine which messages to send, schedule the best time
  to deliver the messages, and then track the results of your campaign.Targeted push
  notifications based on app usage trends and user behavior have become a popular
  approach for mobile app user engagement because response rates are often several
  times higher than tradition email marketing campaigns. By using targeted push notifications,
  you can increase message relevance and effectiveness, measure engagement, and continually
  improve your campaigns.Getting started with Amazon Pinpoint is easy. First, AWS
  Mobile Hub guides you through the process to integrate the AWS Mobile SDK with your
  app. Next, you define your target segments, campaign message, and specify the delivery
  schedule. Once your campaign is running, Pinpoint provides metrics so you can run
  analytics and track the impact of your campaign.With Amazon Pinpoint, there are
  no upfront setup costs, and no fixed monthly cost. You only pay for the number of
  users your campaign targets, the messages you send, and the events you collect,
  so you can start small and scale as your application grows.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
x-kinRank: "10"
x-alexaRank: "0"
tags: Campaign
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Pinpoint API - Get Campaigns
  x-api-slug: appsapplicationidcampaigns-get
  description: Campaigns are messaging initiatives that engage specific segments of
    end users. The information represented by this resource includes the segment that
    the campaign reaches out to, the message that it delivers, and the schedule on
    which it runs. You can use this resource to look up, create, update, or delete
    campaigns.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaigns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaigns-get-openapi.md
- name: AWS Pinpoint API - Add Campaign
  x-api-slug: appsapplicationidcampaigns-put
  description: Use the POST method to create or update a campaign.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaigns-put-openapi.md
- name: AWS Pinpoint API - Campaign Instance
  x-api-slug: appsapplicationidcampaignscampaignid-get
  description: Use the GET method to request information about a campaign.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaignscampaignid-get-openapi.md
- name: AWS Pinpoint API - Update Campaign Instance
  x-api-slug: appsapplicationidcampaignscampaignid-put
  description: Use the PUT method to update a campaign.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaignscampaignid-put-openapi.md
- name: AWS Pinpoint API - Delete Campaign Instance
  x-api-slug: appsapplicationidcampaignscampaignid-delete
  description: Use the DELETE method to delete a campaign.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaignscampaignid-delete-openapi.md
- name: AWS Pinpoint API - Campaign Activities
  x-api-slug: appsapplicationidcampaignscampaignidactivities-get
  description: Returns information about the activity performed by a campaign, such
    as the time during which the campaign ran and the number of endpoints to which
    it delivered messages. You can use this resource to look up activity information
    by app ID and campaign ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaignscampaignidactivities-get-openapi.md
- name: AWS Pinpoint API - Campaign Versions List
  x-api-slug: appsapplicationidcampaignscampaignidversions-get
  description: Use the GET method to request information about your campaign versions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaignscampaignidversions-get-openapi.md
- name: AWS Pinpoint API - Campaign Version Instance
  x-api-slug: appsapplicationidcampaignscampaignidversionsversion-get
  description: Use the GET method to request information about a campaign version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-pinpoint.jpg
  humanURL: https://aws.amazon.com/pinpoint/
  baseURL: :///
  tags: Amazon Web Services, Mobile, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API, Marketing, Marketing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/campaign/master/_listings/aws-pinpoint/appsapplicationidcampaignscampaignidversionsversion-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.opsworks.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.pinpoint.stack.network
- type: x-blog
  url: https://aws.amazon.com/blogs/aws/amazon-pinpoint-hit-your-targets-with-aws/
- type: x-documentation
  url: http://docs.aws.amazon.com/pinpoint/latest/apireference/welcome.html
- type: x-faq
  url: https://aws.amazon.com/pinpoint/faqs/
- type: x-pricing
  url: https://aws.amazon.com/pinpoint/pricing/
- type: x-website
  url: https://aws.amazon.com/pinpoint/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---