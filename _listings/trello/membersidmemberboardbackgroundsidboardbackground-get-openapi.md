---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Members Boardbackgrounds Boardbackground
  description: Get members boardbackgrounds boardbackground.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards:
    post:
      summary: Post Boards
      description: Post boards.
      operationId: addBoards
      x-api-path-slug: boards-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards to be added
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
  /boards/{idBoard}:
    get:
      summary: Get Boards
      description: Get boards.
      operationId: getBoardsByIdBoard
      x-api-path-slug: boardsidboard-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_display
        description: true or false
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_format
        description: 'One of: count, list or minimal'
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: actions_since
        description: A date, null or lastView
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: action_member
        description: true or false
      - in: query
        name: action_memberCreator
        description: true or false
      - in: query
        name: action_memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: action_member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: boardStars
        description: 'One of: mine or none'
      - in: query
        name: cards
        description: 'One of: all, closed, none, open or visible'
      - in: query
        name: card_attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: card_attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: card_checklists
        description: 'One of: all or none'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: card_stickers
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: checklist_fields
        description: 'all or a comma-separated list of: idBoard, idCard, name or pos'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: labels
        description: 'One of: all or none'
      - in: query
        name: labels_limit
        description: a number from 0 to 1000
      - in: query
        name: label_fields
        description: 'all or a comma-separated list of: color, idBoard, name or uses'
      - in: query
        name: lists
        description: 'One of: all, closed, none or open'
      - in: query
        name: list_fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: members
        description: 'One of: admins, all, none, normal or owners'
      - in: query
        name: memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: memberships_member
        description: true or false
      - in: query
        name: memberships_member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: membersInvited
        description: 'One of: admins, all, none, normal or owners'
      - in: query
        name: membersInvited_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: myPrefs
        description: true or false
      - in: query
        name: organization
        description: true or false
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: organization_memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
    put:
      summary: Put Boards
      description: Put boards.
      operationId: updateBoardsByIdBoard
      x-api-path-slug: boardsidboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
  /boards/{idBoard}/actions:
    get:
      summary: Get Boards Actions
      description: Get boards actions.
      operationId: getBoardsActionsByIdBoard
      x-api-path-slug: boardsidboardactions-get
      parameters:
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: display
        description: true or false
      - in: query
        name: entities
        description: true or false
      - in: query
        name: fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: format
        description: 'One of: count, list or minimal'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: idModels
        description: Only return actions related to these model ids
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 0 to 1000
      - in: query
        name: member
        description: true or false
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: page
        description: Page * limit must be less than 1000
      - in: query
        name: since
        description: A date, null or lastView
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Actions
  /boards/{idBoard}/boardStars:
    get:
      summary: Get Boards Boardstars
      description: Get boards boardstars.
      operationId: getBoardsBoardStarsByIdBoard
      x-api-path-slug: boardsidboardboardstars-get
      parameters:
      - in: query
        name: filter
        description: 'One of: mine or none'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Boardstars
  /boards/{idBoard}/calendarKey/generate:
    post:
      summary: Post Boards Calendarkey Generate
      description: Post boards calendarkey generate.
      operationId: addBoardsCalendarKeyGenerateByIdBoard
      x-api-path-slug: boardsidboardcalendarkeygenerate-post
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Calendarkey
      - Generate
  /boards/{idBoard}/cards:
    get:
      summary: Get Boards Cards
      description: Get boards cards.
      operationId: getBoardsCardsByIdBoard
      x-api-path-slug: boardsidboardcards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 1000
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: since
        description: A date, or null
      - in: query
        name: stickers
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
  /boards/{idBoard}/cards/{filter}:
    get:
      summary: Get Boards Cards Filter
      description: Get boards cards filter.
      operationId: getBoardsCardsByIdBoardByFilter
      x-api-path-slug: boardsidboardcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
      - Filter
  /boards/{idBoard}/cards/{idCard}:
    get:
      summary: Get Boards Cards
      description: Get boards cards.
      operationId: getBoardsCardsByIdBoardByIdCard
      x-api-path-slug: boardsidboardcardsidcard-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_display
        description: true or false
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: action_memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checkItemState_fields
        description: 'all or a comma-separated list of: idCheckItem or state'
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: checklist_fields
        description: 'all or a comma-separated list of: idBoard, idCard, name or pos'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idCard
        description: idCard
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: labels
        description: true or false
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
  /boards/{idBoard}/checklists:
    get:
      summary: Get Boards Checklists
      description: Get boards checklists.
      operationId: getBoardsChecklistsByIdBoard
      x-api-path-slug: boardsidboardchecklists-get
      parameters:
      - in: query
        name: cards
        description: 'One of: all, closed, none, open or visible'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: checkItems
        description: 'One of: all or none'
      - in: query
        name: checkItem_fields
        description: 'all or a comma-separated list of: name, nameData, pos, state
          or type'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: idBoard, idCard, name or pos'
      - in: query
        name: filter
        description: 'One of: all or none'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Checklists
    post:
      summary: Post Boards Checklists
      description: Post boards checklists.
      operationId: addBoardsChecklistsByIdBoard
      x-api-path-slug: boardsidboardchecklists-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Checklists to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Checklists
  /boards/{idBoard}/closed:
    put:
      summary: Put Boards Closed
      description: Put boards closed.
      operationId: updateBoardsClosedByIdBoard
      x-api-path-slug: boardsidboardclosed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Closed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Closed
  /boards/{idBoard}/deltas:
    get:
      summary: Get Boards Deltas
      description: Get boards deltas.
      operationId: getBoardsDeltasByIdBoard
      x-api-path-slug: boardsidboarddeltas-get
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: ixLastUpdate
        description: a number from -1 to Infinity
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: tags
        description: A valid tag for subscribing
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Deltas
  /boards/{idBoard}/desc:
    put:
      summary: Put Boards Desc
      description: Put boards desc.
      operationId: updateBoardsDescByIdBoard
      x-api-path-slug: boardsidboarddesc-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Desc to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Desc
  /boards/{idBoard}/emailKey/generate:
    post:
      summary: Post Boards Emailkey Generate
      description: Post boards emailkey generate.
      operationId: addBoardsEmailKeyGenerateByIdBoard
      x-api-path-slug: boardsidboardemailkeygenerate-post
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Emailkey
      - Generate
  /boards/{idBoard}/idOrganization:
    put:
      summary: Put Boards Organization
      description: Put boards organization.
      operationId: updateBoardsIdOrganizationByIdBoard
      x-api-path-slug: boardsidboardidorganization-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Id Organization to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Organization
  /boards/{idBoard}/labelNames/blue:
    put:
      summary: Put Boards Label Names Blue
      description: Put boards label names blue.
      operationId: updateBoardsLabelNamesBlueByIdBoard
      x-api-path-slug: boardsidboardlabelnamesblue-put
      parameters:
      - in: body
        name: body
        description: Attributes of Label Names Blue to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Label
      - Names
      - Blue
  /boards/{idBoard}/labelNames/green:
    put:
      summary: Put Boards Label Names Green
      description: Put boards label names green.
      operationId: updateBoardsLabelNamesGreenByIdBoard
      x-api-path-slug: boardsidboardlabelnamesgreen-put
      parameters:
      - in: body
        name: body
        description: Attributes of Label Names Green to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Label
      - Names
      - Green
  /boards/{idBoard}/labelNames/orange:
    put:
      summary: Put Boards Label Names Orange
      description: Put boards label names orange.
      operationId: updateBoardsLabelNamesOrangeByIdBoard
      x-api-path-slug: boardsidboardlabelnamesorange-put
      parameters:
      - in: body
        name: body
        description: Attributes of Label Names Orange to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Label
      - Names
      - Orange
  /boards/{idBoard}/labelNames/purple:
    put:
      summary: Put Boards Label Names Purple
      description: Put boards label names purple.
      operationId: updateBoardsLabelNamesPurpleByIdBoard
      x-api-path-slug: boardsidboardlabelnamespurple-put
      parameters:
      - in: body
        name: body
        description: Attributes of Label Names Purple to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Label
      - Names
      - Purple
  /boards/{idBoard}/labelNames/red:
    put:
      summary: Put Boards Label Names Red
      description: Put boards label names red.
      operationId: updateBoardsLabelNamesRedByIdBoard
      x-api-path-slug: boardsidboardlabelnamesred-put
      parameters:
      - in: body
        name: body
        description: Attributes of Label Names Red to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Label
      - Names
      - Red
  /boards/{idBoard}/labelNames/yellow:
    put:
      summary: Put Boards Label Names Yellow
      description: Put boards label names yellow.
      operationId: updateBoardsLabelNamesYellowByIdBoard
      x-api-path-slug: boardsidboardlabelnamesyellow-put
      parameters:
      - in: body
        name: body
        description: Attributes of Label Names Yellow to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Label
      - Names
      - Yellow
  /boards/{idBoard}/labels:
    get:
      summary: Get Boards Labels
      description: Get boards labels.
      operationId: getBoardsLabelsByIdBoard
      x-api-path-slug: boardsidboardlabels-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: color, idBoard, name or uses'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 0 to 1000
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Labels
    post:
      summary: Post Boards Labels
      description: Post boards labels.
      operationId: addBoardsLabelsByIdBoard
      x-api-path-slug: boardsidboardlabels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Labels to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Labels
  /boards/{idBoard}/labels/{idLabel}:
    get:
      summary: Get Boards Labels Label
      description: Get boards labels label.
      operationId: getBoardsLabelsByIdBoardByIdLabel
      x-api-path-slug: boardsidboardlabelsidlabel-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: color, idBoard, name or uses'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idLabel
        description: idLabel
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Labels
      - Label
  /boards/{idBoard}/lists:
    get:
      summary: Get Boards Lists
      description: Get boards lists.
      operationId: getBoardsListsByIdBoard
      x-api-path-slug: boardsidboardlists-get
      parameters:
      - in: query
        name: cards
        description: 'One of: all, closed, none, open or visible'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: filter
        description: 'One of: all, closed, none or open'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
    post:
      summary: Post Boards Lists
      description: Post boards lists.
      operationId: addBoardsListsByIdBoard
      x-api-path-slug: boardsidboardlists-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Lists to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
  /boards/{idBoard}/lists/{filter}:
    get:
      summary: Get Boards Lists Filter
      description: Get boards lists filter.
      operationId: getBoardsListsByIdBoardByFilter
      x-api-path-slug: boardsidboardlistsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
      - Filter
  /boards/{idBoard}/markAsViewed:
    post:
      summary: Post Boards Markasviewed
      description: Post boards markasviewed.
      operationId: addBoardsMarkAsViewedByIdBoard
      x-api-path-slug: boardsidboardmarkasviewed-post
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Markasviewed
  /boards/{idBoard}/members:
    get:
      summary: Get Boards Members
      description: Get boards members.
      operationId: getBoardsMembersByIdBoard
      x-api-path-slug: boardsidboardmembers-get
      parameters:
      - in: query
        name: activity
        description: true or false ; works for premium organizations only
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: filter
        description: 'One of: admins, all, none, normal or owners'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
    put:
      summary: Put Boards Members
      description: Put boards members.
      operationId: updateBoardsMembersByIdBoard
      x-api-path-slug: boardsidboardmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
  /boards/{idBoard}/members/{filter}:
    get:
      summary: Get Boards Members Filter
      description: Get boards members filter.
      operationId: getBoardsMembersByIdBoardByFilter
      x-api-path-slug: boardsidboardmembersfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
      - Filter
  /boards/{idBoard}/members/{idMember}:
    delete:
      summary: Delete Boards Members
      description: Delete boards members.
      operationId: deleteBoardsMembersByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmember-delete
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
    put:
      summary: Put Boards Members
      description: Put boards members.
      operationId: updateBoardsMembersByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmember-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
  /boards/{idBoard}/members/{idMember}/cards:
    get:
      summary: Get Boards Members Cards
      description: Get boards members cards.
      operationId: getBoardsMembersCardsByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmembercards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: list
        description: true or false
      - in: query
        name: list_fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
      - Cards
  /boards/{idBoard}/membersInvited:
    get:
      summary: Get Boards Membersinvited
      description: Get boards membersinvited.
      operationId: getBoardsMembersInvitedByIdBoard
      x-api-path-slug: boardsidboardmembersinvited-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Membersinvited
  /boards/{idBoard}/membersInvited/{field}:
    get:
      summary: Get Boards Membersinvited Field
      description: Get boards membersinvited field.
      operationId: getBoardsMembersInvitedByIdBoardByField
      x-api-path-slug: boardsidboardmembersinvitedfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Membersinvited
      - Field
  /boards/{idBoard}/memberships:
    get:
      summary: Get Boards Memberships
      description: Get boards memberships.
      operationId: getBoardsMembershipsByIdBoard
      x-api-path-slug: boardsidboardmemberships-get
      parameters:
      - in: query
        name: filter
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
  /boards/{idBoard}/memberships/{idMembership}:
    get:
      summary: Get Boards Memberships
      description: Get boards memberships.
      operationId: getBoardsMembershipsByIdBoardByIdMembership
      x-api-path-slug: boardsidboardmembershipsidmembership-get
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMembership
        description: idMembership
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
    put:
      summary: Put Boards Memberships
      description: Put boards memberships.
      operationId: updateBoardsMembershipsByIdBoardByIdMembership
      x-api-path-slug: boardsidboardmembershipsidmembership-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Memberships to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMembership
        description: idMembership
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
  /boards/{idBoard}/myPrefs:
    get:
      summary: Get Boards My Preferences
      description: Get boards my preferences.
      operationId: getBoardsMyPrefsByIdBoard
      x-api-path-slug: boardsidboardmyprefs-get
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
  /boards/{idBoard}/myPrefs/emailPosition:
    put:
      summary: Put Boards My Preferences Emailposition
      description: Put boards my preferences emailposition.
      operationId: updateBoardsMyPrefsEmailPositionByIdBoard
      x-api-path-slug: boardsidboardmyprefsemailposition-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Email Position to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Emailposition
  /boards/{idBoard}/myPrefs/idEmailList:
    put:
      summary: Put Boards My Preferences Emaillist
      description: Put boards my preferences emaillist.
      operationId: updateBoardsMyPrefsIdEmailListByIdBoard
      x-api-path-slug: boardsidboardmyprefsidemaillist-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Id Email List to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Emaillist
  /boards/{idBoard}/myPrefs/showListGuide:
    put:
      summary: Put Boards My Preferences Showlistgue
      description: Put boards my preferences showlistgue.
      operationId: updateBoardsMyPrefsShowListGuideByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowlistguide-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show List Guide to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Showlistgue
  /boards/{idBoard}/myPrefs/showSidebar:
    put:
      summary: Put Boards My Preferences Show Sidebar
      description: Put boards my preferences show sidebar.
      operationId: updateBoardsMyPrefsShowSidebarByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebar-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebar
  /boards/{idBoard}/myPrefs/showSidebarActivity:
    put:
      summary: Put Boards My Preferences Show Sidebar Activity
      description: Put boards my preferences show sidebar activity.
      operationId: updateBoardsMyPrefsShowSidebarActivityByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebaractivity-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar Activity to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebar
      - Activity
  /boards/{idBoard}/myPrefs/showSidebarBoardActions:
    put:
      summary: Put Boards My Preferences Show Sidebar Board Actions
      description: Put boards my preferences show sidebar board actions.
      operationId: updateBoardsMyPrefsShowSidebarBoardActionsByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebarboardactions-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar Board Actions to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebar
      - Board
      - Actions
  /boards/{idBoard}/myPrefs/showSidebarMembers:
    put:
      summary: Put Boards My Preferences Show Sidebarmembers
      description: Put boards my preferences show sidebarmembers.
      operationId: updateBoardsMyPrefsShowSidebarMembersByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebarmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebarmembers
  /boards/{idBoard}/name:
    put:
      summary: Put Boards Name
      description: Put boards name.
      operationId: updateBoardsNameByIdBoard
      x-api-path-slug: boardsidboardname-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Name to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Name
  /boards/{idBoard}/organization:
    get:
      summary: Get Boards Organization
      description: Get boards organization.
      operationId: getBoardsOrganizationByIdBoard
      x-api-path-slug: boardsidboardorganization-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Organization
  /boards/{idBoard}/organization/{field}:
    get:
      summary: Get Boards Organization Field
      description: Get boards organization field.
      operationId: getBoardsOrganizationByIdBoardByField
      x-api-path-slug: boardsidboardorganizationfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Organization
      - Field
  /boards/{idBoard}/powerUps:
    post:
      summary: Post Boards Powerups
      description: Post boards powerups.
      operationId: addBoardsPowerUpsByIdBoard
      x-api-path-slug: boardsidboardpowerups-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Power Ups to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Powerups
  /boards/{idBoard}/powerUps/{powerUp}:
    delete:
      summary: Delete Boards Powerups Powerup
      description: Delete boards powerups powerup.
      operationId: deleteBoardsPowerUpsByIdBoardByPowerUp
      x-api-path-slug: boardsidboardpowerupspowerup-delete
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: powerUp
        description: powerUp
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Powerups
      - Powerup
  /boards/{idBoard}/prefs/background:
    put:
      summary: Put Boards Preferences Background
      description: Put boards preferences background.
      operationId: updateBoardsPrefsBackgroundByIdBoard
      x-api-path-slug: boardsidboardprefsbackground-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Background to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Background
  /boards/{idBoard}/prefs/calendarFeedEnabled:
    put:
      summary: Put Boards Preferences Calendar Feed Enabled
      description: Put boards preferences calendar feed enabled.
      operationId: updateBoardsPrefsCalendarFeedEnabledByIdBoard
      x-api-path-slug: boardsidboardprefscalendarfeedenabled-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Calendar Feed Enabled to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Calendar
      - Feed
      - Enabled
  /boards/{idBoard}/prefs/cardAging:
    put:
      summary: Put Boards Preferences Cardaging
      description: Put boards preferences cardaging.
      operationId: updateBoardsPrefsCardAgingByIdBoard
      x-api-path-slug: boardsidboardprefscardaging-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Card Aging to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Cardaging
  /boards/{idBoard}/prefs/cardCovers:
    put:
      summary: Put Boards Preferences Cardcovers
      description: Put boards preferences cardcovers.
      operationId: updateBoardsPrefsCardCoversByIdBoard
      x-api-path-slug: boardsidboardprefscardcovers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Card Covers to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Cardcovers
  /boards/{idBoard}/prefs/comments:
    put:
      summary: Put Boards Preferences Comments
      description: Put boards preferences comments.
      operationId: updateBoardsPrefsCommentsByIdBoard
      x-api-path-slug: boardsidboardprefscomments-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Comments to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Comments
  /boards/{idBoard}/prefs/invitations:
    put:
      summary: Put Boards Preferences Invitations
      description: Put boards preferences invitations.
      operationId: updateBoardsPrefsInvitationsByIdBoard
      x-api-path-slug: boardsidboardprefsinvitations-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Invitations to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Invitations
  /boards/{idBoard}/prefs/permissionLevel:
    put:
      summary: Put Boards Preferences Permissionlevel
      description: Put boards preferences permissionlevel.
      operationId: updateBoardsPrefsPermissionLevelByIdBoard
      x-api-path-slug: boardsidboardprefspermissionlevel-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Permission Level to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Permissionlevel
  /boards/{idBoard}/prefs/selfJoin:
    put:
      summary: Put Boards Preferences Selfjoin
      description: Put boards preferences selfjoin.
      operationId: updateBoardsPrefsSelfJoinByIdBoard
      x-api-path-slug: boardsidboardprefsselfjoin-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Self Join to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Selfjoin
  /boards/{idBoard}/prefs/voting:
    put:
      summary: Put Boards Preferences Voting
      description: Put boards preferences voting.
      operationId: updateBoardsPrefsVotingByIdBoard
      x-api-path-slug: boardsidboardprefsvoting-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Voting to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Voting
  /boards/{idBoard}/subscribed:
    put:
      summary: Put Boards Subscribed
      description: Put boards subscribed.
      operationId: updateBoardsSubscribedByIdBoard
      x-api-path-slug: boardsidboardsubscribed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Subscribed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Subscribed
  /boards/{idBoard}/{field}:
    get:
      summary: Get Boards Field
      description: Get boards field.
      operationId: getBoardsByIdBoardByField
      x-api-path-slug: boardsidboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Field
  /members/{idMember}/boards:
    get:
      summary: Get Members Boards
      description: Get members boards.
      operationId: getMembersBoardsByIdMember
      x-api-path-slug: membersidmemberboards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_format
        description: 'One of: count, list or minimal'
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: actions_since
        description: A date, null or lastView
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: closed, members, open, organization,
          pinned, public, starred or unpinned'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: lists
        description: 'One of: all, closed, none or open'
      - in: query
        name: memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: organization
        description: true or false
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boards
  /members/{idMember}/boards/{filter}:
    get:
      summary: Get Members Boards Filter
      description: Get members boards filter.
      operationId: getMembersBoardsByIdMemberByFilter
      x-api-path-slug: membersidmemberboardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boards
      - Filter
  /organizations/{idOrg}/boards:
    get:
      summary: Get Organizations Boards
      description: Get organizations boards.
      operationId: getOrganizationsBoardsByIdOrg
      x-api-path-slug: organizationsidorgboards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_format
        description: 'One of: count, list or minimal'
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: actions_since
        description: A date, null or lastView
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: closed, members, open, organization,
          pinned, public, starred or unpinned'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: lists
        description: 'One of: all, closed, none or open'
      - in: query
        name: memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: organization
        description: true or false
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Boards
  /organizations/{idOrg}/boards/{filter}:
    get:
      summary: Get Organizations Boards Filter
      description: Get organizations boards filter.
      operationId: getOrganizationsBoardsByIdOrgByFilter
      x-api-path-slug: organizationsidorgboardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Boards
      - Filter
  /actions/{idAction}/board:
    get:
      summary: Get Actions Board
      description: Get actions board.
      operationId: getActionsBoardByIdAction
      x-api-path-slug: actionsidactionboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Board
  /actions/{idAction}/board/{field}:
    get:
      summary: Get Actions Board Field
      description: Get actions board field.
      operationId: getActionsBoardByIdActionByField
      x-api-path-slug: actionsidactionboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Board
      - Field
  /cards/{idCard}/board:
    get:
      summary: Get Cards Board
      description: Get cards board.
      operationId: getCardsBoardByIdCard
      x-api-path-slug: cardsidcardboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Board
  /cards/{idCard}/board/{field}:
    get:
      summary: Get Cards Board Field
      description: Get cards board field.
      operationId: getCardsBoardByIdCardByField
      x-api-path-slug: cardsidcardboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Board
      - Field
  /cards/{idCard}/idBoard:
    put:
      summary: Put Cards Board
      description: Put cards board.
      operationId: updateCardsIdBoardByIdCard
      x-api-path-slug: cardsidcardidboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Board to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Board
  /checklists/{idChecklist}/board:
    get:
      summary: Get Checklists Board
      description: Get checklists board.
      operationId: getChecklistsBoardByIdChecklist
      x-api-path-slug: checklistsidchecklistboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idChecklist
        description: idChecklist
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Checklists
      - Board
  /checklists/{idChecklist}/board/{field}:
    get:
      summary: Get Checklists Board Field
      description: Get checklists board field.
      operationId: getChecklistsBoardByIdChecklistByField
      x-api-path-slug: checklistsidchecklistboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idChecklist
        description: idChecklist
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Checklists
      - Board
      - Field
  /labels/{idLabel}/board:
    get:
      summary: Get Labels Label Board
      description: Get labels label board.
      operationId: getLabelsBoardByIdLabel
      x-api-path-slug: labelsidlabelboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idLabel
        description: idLabel
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Labels
      - Label
      - Board
  /labels/{idLabel}/board/{field}:
    get:
      summary: Get Labels Label Board Field
      description: Get labels label board field.
      operationId: getLabelsBoardByIdLabelByField
      x-api-path-slug: labelsidlabelboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idLabel
        description: idLabel
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Labels
      - Label
      - Board
      - Field
  /lists/{idList}/board:
    get:
      summary: Get Lists List Board
      description: Get lists list board.
      operationId: getListsBoardByIdList
      x-api-path-slug: listsidlistboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Board
  /lists/{idList}/board/{field}:
    get:
      summary: Get Lists List Board Field
      description: Get lists list board field.
      operationId: getListsBoardByIdListByField
      x-api-path-slug: listsidlistboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Board
      - Field
  /lists/{idList}/idBoard:
    put:
      summary: Put Lists List Board
      description: Put lists list board.
      operationId: updateListsIdBoardByIdList
      x-api-path-slug: listsidlistidboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Id Board to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Board
  /members/{idMember}/boardStars/{idBoardStar}/idBoard:
    put:
      summary: Put Members Boardstars Board
      description: Put members boardstars board.
      operationId: updateMembersBoardStarsIdBoardByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstaridboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars Id Board to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
      - Board
  /notifications/{idNotification}/board:
    get:
      summary: Get Notifications Notification Board
      description: Get notifications notification board.
      operationId: getNotificationsBoardByIdNotification
      x-api-path-slug: notificationsidnotificationboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Board
  /notifications/{idNotification}/board/{field}:
    get:
      summary: Get Notifications Notification Board Field
      description: Get notifications notification board field.
      operationId: getNotificationsBoardByIdNotificationByField
      x-api-path-slug: notificationsidnotificationboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - Board
      - Field
  /members/{idMember}/boardBackgrounds/{idBoardBackground}:
    delete:
      summary: Delete Members Boardbackgrounds Boardbackground
      description: Delete members boardbackgrounds boardbackground.
      operationId: deleteMembersBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmemberboardbackgroundsidboardbackground-delete
      parameters:
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
      - Boardbackground
    get:
      summary: Get Members Boardbackgrounds Boardbackground
      description: Get members boardbackgrounds boardbackground.
      operationId: getMembersBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmemberboardbackgroundsidboardbackground-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: brightness, fullSizeUrl, scaled
          or tile'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
      - Boardbackground
    put:
      summary: Put Members Boardbackgrounds Boardbackground
      description: Put members boardbackgrounds boardbackground.
      operationId: updateMembersBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmemberboardbackgroundsidboardbackground-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Backgrounds to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
      - Boardbackground
  /members/{idMember}/customBoardBackgrounds/{idBoardBackground}:
    delete:
      summary: Delete Members Customboardbackgrounds Boardbackground
      description: Delete members customboardbackgrounds boardbackground.
      operationId: deleteMembersCustomBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmembercustomboardbackgroundsidboardbackground-delete
      parameters:
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
      - Boardbackground
    get:
      summary: Get Members Customboardbackgrounds Boardbackground
      description: Get members customboardbackgrounds boardbackground.
      operationId: getMembersCustomBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmembercustomboardbackgroundsidboardbackground-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: brightness, fullSizeUrl, scaled
          or tile'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
      - Boardbackground
    put:
      summary: Put Members Customboardbackgrounds Boardbackground
      description: Put members customboardbackgrounds boardbackground.
      operationId: updateMembersCustomBoardBackgroundsByIdMemberByIdBoardBackground
      x-api-path-slug: membersidmembercustomboardbackgroundsidboardbackground-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Custom Board Backgrounds to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardBackground
        description: idBoardBackground
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Customboardbackgrounds
      - Boardbackground
  /members/{idMember}/boardBackgrounds:
    get:
      summary: Get Members Boardbackgrounds
      description: Get members boardbackgrounds.
      operationId: getMembersBoardBackgroundsByIdMember
      x-api-path-slug: membersidmemberboardbackgrounds-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all, custom, default, none or premium'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
    post:
      summary: Post Members Boardbackgrounds
      description: Post members boardbackgrounds.
      operationId: addMembersBoardBackgroundsByIdMember
      x-api-path-slug: membersidmemberboardbackgrounds-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Backgrounds to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardbackgrounds
  /members/{idMember}/boardsInvited:
    get:
      summary: Get Members Boardsinvited
      description: Get members boardsinvited.
      operationId: getMembersBoardsInvitedByIdMember
      x-api-path-slug: membersidmemberboardsinvited-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardsinvited
  /members/{idMember}/boardsInvited/{field}:
    get:
      summary: Get Members Boardsinvited Field
      description: Get members boardsinvited field.
      operationId: getMembersBoardsInvitedByIdMemberByField
      x-api-path-slug: membersidmemberboardsinvitedfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardsinvited
      - Field
  /members/{idMember}/boardStars:
    get:
      summary: Get Members Boardstars
      description: Get members boardstars.
      operationId: getMembersBoardStarsByIdMember
      x-api-path-slug: membersidmemberboardstars-get
      parameters:
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
    post:
      summary: Post Members Boardstars
      description: Post members boardstars.
      operationId: addMembersBoardStarsByIdMember
      x-api-path-slug: membersidmemberboardstars-post
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
  /members/{idMember}/boardStars/{idBoardStar}:
    delete:
      summary: Delete Members Boardstars
      description: Delete members boardstars.
      operationId: deleteMembersBoardStarsByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstar-delete
      parameters:
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
    get:
      summary: Get Members Boardstars
      description: Get members boardstars.
      operationId: getMembersBoardStarsByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstar-get
      parameters:
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
    put:
      summary: Put Members Boardstars
      description: Put members boardstars.
      operationId: updateMembersBoardStarsByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstar-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
  /members/{idMember}/boardStars/{idBoardStar}/pos:
    put:
      summary: Put Members Boardstars Pos
      description: Put members boardstars pos.
      operationId: updateMembersBoardStarsPosByIdMemberByIdBoardStar
      x-api-path-slug: membersidmemberboardstarsidboardstarpos-put
      parameters:
      - in: body
        name: body
        description: Attributes of Members Board Stars Pos to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoardStar
        description: idBoardStar
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Boardstars
      - Pos
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/org:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Org
      description: Put organizations preferences boardvisibilityrestrict org.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictOrgByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictorg-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Org
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/private:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Private
      description: Put organizations preferences boardvisibilityrestrict private.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictPrivateByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictprivate-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Private
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/public:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Public
      description: Put organizations preferences boardvisibilityrestrict public.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictPublicByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictpublic-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Public
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