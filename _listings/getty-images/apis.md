---
name: Getty Images
x-slug: getty-images
description: Find high resolution royalty-free images, editorial stock photos, vector
  art, video footage clips and stock music licensing at the richest image search photo
  library online.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
x-kinRank: "8"
x-alexaRank: "1939"
tags: Boards
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Get All Boards
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to retrieve all Boards available for a user.\r\n\r\nYou'll need
    an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boards-get-openapi.md
- name: Getty Images Create Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to create a Board by a specific id.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n**NOTE:** *The
    input to this endpoint is not sanitized in any way, so it is the responsibility
    of the client to ensure that it is properly formatted and guards against malicious
    data (for example cross-site scripting attacks or HTML injection) when accessing
    the data.*"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Images,Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boards-post-openapi.md
- name: Getty Images Delete Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to delete a Board by a specific id.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-id-delete-openapi.md
- name: Getty Images Get Board Assets
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to retrieve a Board by a specific id.\r\n\r\nYou'll need an
    API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-id-get-openapi.md
- name: Getty Images Update Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to update a Board by a specific id.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key.\r\n\r\n**NOTE:** *The
    input to this endpoint is not sanitized in any way, so it is the responsibility
    of the client to ensure that it is properly formatted and guards against malicious
    data (for example cross-site scripting attacks or HTML injection) when accessing
    the data.*"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Images,Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-id-put-openapi.md
- name: Getty Images Remove Assets From Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to remove a set of assets from a board.\r\n\r\nYou'll need an API
    key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassets-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassets-delete-openapi.md
- name: Getty Images Add Assets to a Board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to add a set of assets to a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Images,Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassets-put-openapi.md
- name: Getty Images Remove an asset from a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to remove an asset from a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassetsasset-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassetsasset-id-delete-openapi.md
- name: Getty Images Add an asset to a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place.\r\nMore information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to add an asset to a board.\r\n\r\nYou'll need an API key and
    a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Images,Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassetsasset-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idassetsasset-id-put-openapi.md
- name: Getty Images Get comments from a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
    Use this endpoint to retrieve all comments for a specific board.\r\n\r\nYou'll
    need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Images,Boards,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idcomments-get-openapi.md
- name: Getty Images Add a comment to a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to add a comment to a board.\r\n\r\nYou'll need an API key and a
    [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Images,Boards,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idcomments-post-openapi.md
- name: Getty Images Delete a comment from a board
  x-api-slug: getty-images
  description: "Boards are where you collect, curate, collaborate on and manage photo
    and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
    this endpoint to delete a comment from a board.\r\n\r\nYou'll need an API key
    and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
    access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments/{comment_id}
  tags: Images,Boards,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idcommentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/v3boardsboard-idcommentscomment-id-delete-openapi.md
- name: Getty Images
  x-api-slug: getty-images
  description: Find high resolution royalty-free images, editorial stock photos, vector
    art, video footage clips and stock music licensing at the richest image search
    photo library online.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/getty-images/openapi.md
x-common:
- type: x-authentication
  url: https://github.com/gettyimages/connect#authentication
- type: x-base
  url: https://connect.gettyimages.com/
- type: x--net-sdk
  url: https://github.com/gettyimages/connect_sdk_csharp
- type: x-crunchbase
  url: https://crunchbase.com/organization/gettyimages
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ge-tt
- type: x-developer
  url: http://api.gettyimages.com/
- type: x-documentation
  url: https://api.gettyimages.com/swagger/ui/index.html
- type: x-email
  url: privacy@gettyimages.com
- type: x-email
  url: sales@gettyimages.com
- type: x-email
  url: copyright@gettyimages.com
- type: x-embeddable
  url: https://github.com/gettyimages/connect#oembed
- type: x-forum
  url: http://api.gettyimages.com/forum
- type: x-getting-started
  url: https://github.com/gettyimages/connect#getting-started
- type: x-github
  url: https://github.com/gettyimages
- type: x-java-sdk
  url: https://github.com/gettyimages/connect_sdk_java
- type: x-node-js-sdk
  url: https://github.com/gettyimages/connect_sdk_nodejs
- type: x-objectivec-sdk
  url: https://github.com/gettyimages/connect_sdk_objective-c
- type: x-php-sdk
  url: https://github.com/gettyimages/connect_sdk_php
- type: x-pricing
  url: http://www.gettyimages.com/subscribe
- type: x-ruby-sdk
  url: https://github.com/gettyimages/connect_sdk_ruby
- type: x-twitter
  url: https://twitter.com/GettyImages
- type: x-website
  url: http://www.gettyimages.com/
- type: x-website
  url: http://gettyimages.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---