chatbot
~~~~~~~

modular framework for building telegram bots

DRAFT:

  +---------------------------+
  | network interface adaptor |
  +---------------------------+
               AV
               ||
               VA
  +---------------------------+
  |     message dispatcher    |
  +---------------------------+
               AV
               ||
               VA
     +--------------------------+
   +--------------------------+ |
 +--------------------------+ |-+
 |     message handlers     |-+
 +--------------------------+
               AV
               ||
               VA
     +--------------------------+
   +--------------------------+ |
 +--------------------------+ |-+
 |     action handlers      |-+
 +--------------------------+


* Connection Management
* Session Management
* User Management
* Access Management
* Module Management

User::
  ID -- Unique Identifier for User
  Description -- optional description.
  PrimaryNickname -- Primary Nickname. Must be unique.
  LastNickname -- Nickname last used.
  Aliases -- List of commonly using nicknames for this user
  CreatedTime -- timestamp when user was registered
  LastSeenTime -- timestamp when user last accessed to the bot
  LastActionTime -- timestamp when user last send message to others
  Permissions -- list of permission ids

Group::
  ID -- Uniquie Identifier for Group
  Name -- Uniqie name of group
  Description -- optional text describe primary purpose of this group
  Members -- list of identifiers of users belongs to this group
  Permissions -- list of ids of permissions

Permission::
  ID -- unique identifier for permission
  Description -- text describe 
