### Using Finger

#### The `Finger` command

To 'finger' a user, all you need to do is call `finger <user>@<hostname>` on the command line:

```
[nikdoof@s1] (~) % finger nikdoof@dimension.sh
[dimension.sh]

Plan:
  https://nikdoof.com/now
Pronouns:
  he/him
Projects:
  Furthering the development of dimension.sh
Online.
```

On some servers, finger responds with special output when calling `@<domain>` or `root@<domain>`

```
[nikdoof@s1] (~) % finger @dimension.sh
[dimension.sh]
  __                                                                          __
 /\ \  __                                     __                             /\ \
 \_\ \/\_\    ___ ___      __    ___     ____/\_\    ___     ___         ____\ \ \___
 /'_` \/\ \ /' __` __`\  /'__`\/' _ `\  /',__\/\ \  / __`\ /' _ `\      /',__\\ \  _ `\
/\ \L\ \ \ \/\ \/\ \/\ \/\  __//\ \/\ \/\__, `\ \ \/\ \L\ \/\ \/\ \  __/\__, `\\ \ \ \ \
\ \___,_\ \_\ \_\ \_\ \_\ \____\ \_\ \_\/\____/\ \_\ \____/\ \_\ \_\/\_\/\____/ \ \_\ \_\
 \/__,_ /\/_/\/_/\/_/\/_/\/____/\/_/\/_/\/___/  \/_/\/___/  \/_/\/_/\/_/\/___/   \/_/\/_/


dimension.sh is a shared linux shell system (or pubnix), open to everyone and anyone to
use, learn, and experiment.

If you're interested in joining check out the website: https://dimension.sh
users currently logged in are:

nikdoof  + pts/0        2021-06-03 09:44 00:02      801233
```

#### Customising your Finger responses

On dimension.sh, we have a operating Finger server that is available to the wider internet. You can customize what is returned to the caller with a collection of files in your home directory.

* `.plan` - A free-form text file that can be filled with whatever you want. (see the [Jargon file](http://www.catb.org/jargon/html/P/plan-file.html)).
* `.project` - A file describing your current project.
* `.pronouns` - A file to store your pronouns.


