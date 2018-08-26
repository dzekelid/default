---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Whitelabel Links Default
  description: |-
    **This endpoint allows you to retrieve the default link whitelabel.**

    Default link whitelabel is the actual link whitelabel to be used when sending messages. If there are multiple link whitelabels, the default is determined by the following order:
    <ul>
      <li>Validated link whitelabels marked as "default"</li>
      <li>Legacy link whitelabels (migrated from the whitelabel wizard)</li>
      <li>Default SendGrid link whitelabel (i.e. 100.ct.sendgrid.net)</li>
    </ul>

    Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

    For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /whitelabel/domains/default:
    get:
      summary: Get Whitelabel Domains Default
      description: |-
        **This endpoint allows you to retrieve the default whitelabel for a domain.**

        A domain whitelabel allows you to remove the ???via??? or ???sent on behalf of??? message that your recipients see when they read your emails. Whitelabeling a domain allows you to replace sendgrid.net with your personal sending domain. You will be required to create a subdomain so that SendGrid can generate the DNS records which you must give to your host provider. If you choose to use Automated Security, SendGrid will provide you with 3 CNAME records. If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.

        For more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)

        ## URI Parameters
        | URI Parameter   | Type   | Description  |
        |---|---|---|
        | domain | string  |The domain to find a default domain whitelabel for. |
      operationId: whitelabel.domains.default.get
      x-api-path-slug: whitelabeldomainsdefault-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Domains
      - Default
  /whitelabel/links/default:
    get:
      summary: Get Whitelabel Links Default
      description: |-
        **This endpoint allows you to retrieve the default link whitelabel.**

        Default link whitelabel is the actual link whitelabel to be used when sending messages. If there are multiple link whitelabels, the default is determined by the following order:
        <ul>
          <li>Validated link whitelabels marked as "default"</li>
          <li>Legacy link whitelabels (migrated from the whitelabel wizard)</li>
          <li>Default SendGrid link whitelabel (i.e. 100.ct.sendgrid.net)</li>
        </ul>

        Email link whitelabels allow all of the click-tracked links you send in your emails to include the URL of your domain instead of sendgrid.net.

        For more information, please see our [User Guide](https://sendgrid.com/docs/API_Reference/Web_API_v3/Whitelabel/links.html).
      operationId: whitelabel.links.default.get
      x-api-path-slug: whitelabellinksdefault-get
      parameters:
      - in: query
        name: domain
        description: The domain to match against when finding a corresponding link
          whitelabel
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Links
      - Default
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---