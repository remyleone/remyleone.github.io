---
layout: article
title: Hash in Python
teaser: Useful for tagging
description: Quick snippet to create an hash in python
tags:
  - code
  - python
---

Python 3 is shipped with a hash library. To use it in a script just do
this :

{% highlight python %}

import hashlib
message = "Bonjour"
h = hashlib.sha512()
h.update(message.encode("utf-8"))
print(h.hexdigest())

{% endhighlight %}

Don't forget encoding ;)
