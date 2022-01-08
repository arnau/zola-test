+++
title = "A dive into the  Link header"
description = "This note describes my current understanding of the  Link header as defined\nby the IETF RFC8288."
date = 2019-06-22
+++
A test


```abnf
header = link *(OWS "," OWS link)
link   = "<" target ">" *(OWS ";" OWS param)
param  = name ["=" value]
target = uriref
name   = token
value  = token / quoted-string
```
