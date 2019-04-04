---
title: YANG Groupings for UDP Clients and UDP Servers 
abbrev: Groupings for UDP Clients and Servers
docname: draft-birkholz-netconf-udp-client-server-latest
stand_alone: true
ipr: trust200902
area: Operations and Management
wg: NETCONF Working Group
kw: Internet-Draft
cat: std
pi:
  toc: yes
  sortrefs: yes
  symrefs: yes

author:
- ins: H. Birkholz
  name: Henk Birkholz
  org: Fraunhofer SIT
  abbrev: Fraunhofer SIT
  email: henk.birkholz@sit.fraunhofer.de
  street: Rheinstrasse 75
  code: '64295'
  city: Darmstadt
  country: Germany

normative:
  RFC7950:
  RFC8340:
  RFC6991:

--- abstract

This document defines two YANG modules: the first defines a grouping for configuring a generic UDP client, and the second defines a grouping for configuring a generic UDP server.
It is intended that these groupings will be used by applications using the UDP protocol.

--- middle

# Introduction

This document defines two YANG 1.1 {{RFC7950}} modules: the first defines a grouping for configuring a generic UDP client, and the second defines a grouping for configuring a generic UDP server.
It is intended that these groupings will be used by applications using the UDP protocol.
For instance, these groupings could help define the configuration module for an DTLS-based application.

# Requirements Notation

{::boilerplate bcp14}

# The UDP Client Model

## Tree Diagram

This section provides a tree diagram {{RFC8340}} for the "ietf-udp-client" module.

~~~~
<CODE BEGINS>
; {::include ietf-udp-client.tree}
<CODE ENDS>
~~~~

## Example Usage

~~~~
<CODE BEGINS>
; {::include ietf-udp-client.example}
<CODE ENDS>
~~~~

## YANG Module

This YANG module has normative references to {{RFC6991}}.

~~~~
<CODE BEGINS> file "ietf-udp-server@2019-04-04.yang"
; {::include ietf-udp-server.yang}
<CODE ENDS>
~~~~

# The UDP Server Model

## Tree Diagram

This section provides a tree diagram {{RFC8340}} for the "ietf-udp-server" module.

~~~~
<CODE BEGINS>
; {::include ietf-udp-server.tree}
<CODE ENDS>
~~~~

## Example Usage

~~~~
<CODE BEGINS>
; {::include ietf-udp-server.example}
<CODE ENDS>
~~~~

## YANG Module

This YANG module has normative references to {{RFC6991}}.

~~~~
<CODE BEGINS> file "ietf-udp-server@2019-04-04.yang"
; {::include ietf-udp-server.yang}
<CODE ENDS>
~~~~

# Security Considerations

#  Acknowledgments

#  Change Log

# Contributors

--- back
