# Table of Contents

- [Table of Contents](#table-of-contents)
- [Technical Document for Schema.md](#technical-document-for-schemamd)
  - [Compensation](#compensation)
  - [Social Media](#social-media)
  - [Locations](#locations)
  - [Contacts](#contacts)
- [Filters](#filters)
- [Causes List](#causes-list)

# Technical Document for Schema.md

**IMPORTANT: _Arrays_ cannot be nullable. Make it an empty array `[]`**

- name              : String
- cause             : String
- no_of_volunteers  : Integer
- about             : String
- website           : String
- available_roles   : Array (String)
- scope             : Array (String)
- similar_ngos      : Array (String)
- compensation      : Array ([Compensation](#compensation))
- social_media      : Array ([Social_Media](#social-media))
- locations         : Array ([Locations](#locations))
- contacts          : Array ([Contacts](#contacts))

## Compensation

- position          : String
- type              : String

## Social Media

- type              : String
- url               : String

## Locations

- type              : String
- street_address    : String 
- city              : String
- pin               : Integer
- state             : String
- latitude          : Float
- longitude         : Float

## Contacts

- type              : String
- email             : String
- numbers           : Array (Integer)

# Filters

- Compensation
  - Paid
  - Unpaid
  - Reference (compensation)
- Location
  - States of India (27)
  - Reference (locations.state)
- Cause
  - Cause of NGO (Needs to be listed)
  - Reference (cause)
  - NOTE, Please make a list of all the causes available
- Scope
  - Onsite
  - Online
  - Reference (scope)


# Causes List

> TODO, Please write all the causes here 

> This is what the User will choose from and these values will also be present inside the NGO cause fields
