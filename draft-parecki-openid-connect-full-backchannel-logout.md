---
title: "OpenID Connect Full Back-Channel Logout"
abbrev: "Full Back-Channel Logout"
category: info

docname: draft-parecki-openid-connect-full-backchannel-logout-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
area: AREA
workgroup: OpenID Connect
keyword:
 - logout
 - revocation
venue:
  group: OpenID Connect
  type: Working Group
  mail: openid-specs-ab@lists.openid.net
  arch: https://openid.net
  github: aaronpk/openid-connect-full-backchannel-logout
  latest: https://github.com/aaronpk/openid-connect-full-backchannel-logout

author:
 -
    fullname: Aaron Parecki
    organization: Okta
    email: aaron@parecki.com

normative:
  OpenID:
    title: OpenID Connect Core 1.0
    target: https://openid.net/specs/openid-connect-core-1_0.html
    date: November 8, 2014
    author:
      - ins: N. Sakimura
      - ins: J. Bradley
      - ins: M. Jones
      - ins: B. de Medeiros
      - ins: C. Mortimore
  RFC6749:
  RFC8414:
  IANA.oauth-parameters:

informative:


--- abstract

OpenID Connect 1.0 is an identity layer on top of the OAuth 2.0 {{RFC6749}} protocol. It enables Clients to verify the identity of the End-User based on the authentication performed by an Authorization Server, as well as to obtain basic profile information about the End-User in an interoperable and REST-like manner.

OpenID Connect Back-Channel Logout defines a mechanism for an OP to signal to an RP that a user should be logged out. However, it recommends that refresh tokens issued with the `offline_access` scope SHOULD NOT be revoked.

This specification defines a new back-channel logout request that adds the requirement to revoke all refresh tokens, in addition to terminating the session.


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
