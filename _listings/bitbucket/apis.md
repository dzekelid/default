---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Default
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Repositories Username Repo Slug Default Reviewers
  x-api-slug: bitbucket
  description: |-
    Returns the repository's default reviewers.

    These are the users that are automatically added as reviewers on every
    new pull request that is created.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/default-reviewers
  tags: Repositories, Username, Repo, Slug, Default, Reviewers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Default Reviewers
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug default reviewers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/default-reviewers
  tags: Repositories, Username, Repo, Slug, Default, Reviewers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-parameters-openapi.md
- name: Bitbucket Delete Repositories Username Repo Slug Default Reviewers Target
    Username
  x-api-slug: bitbucket
  description: Delete repositories username repo slug default reviewers target username
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/default-reviewers/{target_username}
  tags: Repositories, Username, Repo, Slug, Default, Reviewers, Target, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-delete-openapi.md
- name: Bitbucket Get Repositories Username Repo Slug Default Reviewers Target Username
  x-api-slug: bitbucket
  description: |-
    Returns the specified reviewer.

    This can be used to test whether a user is among the repository's
    default reviewers list. A 404 indicates that that specified user is not
    a default reviewer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/default-reviewers/{target_username}
  tags: Repositories, Username, Repo, Slug, Default, Reviewers, Target, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-get-openapi.md
- name: Bitbucket Parameters Repositories Username Repo Slug Default Reviewers Target
    Username
  x-api-slug: bitbucket
  description: Parameters repositories username repo slug default reviewers target
    username
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/default-reviewers/{target_username}
  tags: Repositories, Username, Repo, Slug, Default, Reviewers, Target, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-parameters-openapi.md
- name: Bitbucket Update Repositories Username Repo Slug Default Reviewers Target
    Username
  x-api-slug: bitbucket
  description: |-
    Adds the specified user to the repository's list of default
    reviewers.

    This method is idempotent. Adding a user a second time has no effect.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//repositories/{username}/{repo_slug}/default-reviewers/{target_username}
  tags: Repositories, Username, Repo, Slug, Default, Reviewers, Target, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-put-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Default
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/default/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---