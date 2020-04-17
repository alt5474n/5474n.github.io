---
layout: post
title: thingsChange.sh
---

# echo ", Mox" >> thingsChange.conf && ./thingsChange.sh

Been working on updating an Elasticsearch cluster. And old one. A version 1.6 cluster. To version 7.6.2.

Granted this is a long overdue update to this system&#151;don't look at me, I inherited it&#151;but it's incredible how many under-the-hood things change.

Like variables.

I've grep'ed and sed'ed and vimdiff'ed more than a man would ever want to because of constantly finding small variable changes.

Like this...
```javascript
trim => "<>"
```
Becomes:
```javascript
trim_value => "<>"
```

I'm sure there's a logical reason for it all. A necessary evil.

Because afterall:
>"The only constant in life is change.
>&#151;Heraclitus
