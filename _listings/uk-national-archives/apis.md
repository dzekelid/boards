---
name: UK National Archives
x-slug: uk-national-archives
description: The National Archives (TNA) is a non-ministerial government department.
  Its parent department is the Department for Culture, Media and Sport of the United
  Kingdom of Great Britain and Northern Ireland. It is the official archive of the
  UK government and for England and Wales; and guardian of some of the nations most
  iconic documents, dating back more than 1,000 years. There are separate national
  archives for Scotland (the National Records of Scotland) and Northern Ireland (the
  Public Record Office of Northern Ireland).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Boards
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Search API Get Boards
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get all boards that the user participates in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Boards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boards-get-openapi.md
- name: Getty Images Search API Post Boards
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> create a new board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards
  tags: Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boards-post-openapi.md
- name: Getty Images Search API Delete Boards Board
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> delete a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Boards,Board
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-id-delete-openapi.md
- name: Getty Images Search API Get Boards Board
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get assets and metadata for a specific board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Boards,Board
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-id-get-openapi.md
- name: Getty Images Search API Put Boards Board
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> update a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}
  tags: Boards,Board
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-id-put-openapi.md
- name: Getty Images Search API Delete Boards Board Assets
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> remove assets from a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Boards,Board,Assets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idassets-delete-openapi.md
- name: Getty Images Search API Put Boards Board Assets
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add assets to a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets
  tags: Boards,Board,Assets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idassets-put-openapi.md
- name: Getty Images Search API Delete Boards Board Assets Asset
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> remove an asset from a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Boards,Board,Assets,Asset
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idassetsasset-id-delete-openapi.md
- name: Getty Images Search API Put Boards Board Assets Asset
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add an asset to a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/assets/{asset_id}
  tags: Boards,Board,Assets,Asset
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idassetsasset-id-put-openapi.md
- name: Getty Images Search API Get Boards Board Comments
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> get comments from a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Boards,Board,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idcomments-get-openapi.md
- name: Getty Images Search API Post Boards Board Comments
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> add a comment to a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments
  tags: Boards,Board,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idcomments-post-openapi.md
- name: Getty Images Search API Delete Boards Board Comments Comment
  x-api-slug: getty-images-search-api
  description: <b>***beta***</b> delete a comment from a board.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/boards/{board_id}/comments/{comment_id}
  tags: Boards,Board,Comments,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/v3boardsboard-idcommentscomment-id-delete-openapi.md
- name: Getty Images Search API
  x-api-slug: getty-images-search-api
  description: Our set of APIs enable seamless integration of Getty Images expansive
    content, powerful search and rich metadata directly into your internal workflows,
    products and services. With Connects API solutions, you can fully control, customize
    and scale as you grow.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/uk-national-archives.jpeg
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com//
  tags: Boards
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/boards/master/_listings/uk-national-archives/openapi.md
x-common:
- type: x-website
  url: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
- type: x-website
  url: http:///Search
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---