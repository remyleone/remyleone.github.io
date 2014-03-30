---
layout: post
title: Hash in Python
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
