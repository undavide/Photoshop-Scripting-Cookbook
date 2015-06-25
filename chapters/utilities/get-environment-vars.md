---
layout: recipe
title: Get Environment vars
chapter: Template Chapter
---

## Problem
You'd like to access Environment Variables via scripting.

## Solution
You can rely on the `$` utility object function `getenv()`, which accepts a string as a parameter:

{% highlight javascript %}
alert( $.getenv("USERNAME") ); // Davide
{% endhighlight %}

## Discussion
The available arguments of the `getenv` call depend on the platform, for the lists read along.

#### Mac

Open the Terminal and type `printenv`, the records (populated with your own data) will be:
{% highlight console %}
TERM_PROGRAM
TERM
SHELL
TMPDIR
Apple_PubSub_Socket_Render
TERM_PROGRAM_VERSION
TERM_SESSION_ID
USER
SSH_AUTH_SOCK
__CF_USER_TEXT_ENCODING
PATH
PWD
XPC_FLAGS
PS1
XPC_SERVICE_NAME
HOME
SHLVL
LOGNAME
LC_CTYPE
DISPLAY
SECURITYSESSIONID
OLDPWD
{% endhighlight %}

#### PC

Open the Command Prompt and type `set`, the records (populated with your own data) will be:
{% highlight console %}
ALLUSERSPROFILE
APPDATA
CommonProgramFiles
CommonProgramFiles(x86)
CommonProgramW6432
COMPUTERNAME
ComSpec
FP_NO_HOST_CHECK
HOMEDRIVE
HOMEPATH
LOCALAPPDATA
LOGONSERVER
NUMBER_OF_PROCESSORS
OS
Path
PATHEXT
PROCESSOR_ARCHITECTURE
PROCESSOR_IDENTIFIER
PROCESSOR_LEVEL
PROCESSOR_REVISION
ProgramData
ProgramFiles
ProgramFiles(x86)
ProgramW6432
PROMPT
PSModulePath
PUBLIC
SESSIONNAME
SystemDrive
SystemRoot
TEMP
TMP
USERDOMAIN
USERNAME
USERPROFILE
windir
{% endhighlight %}

### References
Credits: AA.VV.

Link: not provided.
