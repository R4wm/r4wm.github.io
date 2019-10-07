---
layout: post
title: TIL: Bash has a ternary
catagories: [programming, bash]
tags: [bash, coding, til]
---

# Bash Parameter Expansion
* so today I learned there is a ternary like thing for bash.

My old way of doing things

```bash
ᚱ@two-fer $ bat -p /tmp/stuff.sh
#!/bin/bash

if [ "$1" ]
then
    echo "One for $1, one for me."
    exit 0
fi

echo "One for you, one for me."


ᚱ@two-fer $ 
ᚱ@two-fer $ /tmp/stuff.sh 
One for you, one for me.
ᚱ@two-fer $ 
ᚱ@two-fer $ /tmp/stuff.sh coolguy
One for coolguy, one for me.
ᚱ@two-fer $ 
```

Applying what I learnt!
```bash
ᚱ@two-fer $ bat -p /tmp/stuff.sh
#!/bin/bash

echo "One for ${1:-you}, one for me."

ᚱ@two-fer $ 
ᚱ@two-fer $ /tmp/stuff.sh coolguy
One for coolguy, one for me.
ᚱ@two-fer $ 
ᚱ@two-fer $ 
ᚱ@two-fer $ /tmp/stuff.sh
One for you, one for me.
ᚱ@two-fer $ 
```
* The above example basically checks to see if the variable is set, if not, the default value will be used.
