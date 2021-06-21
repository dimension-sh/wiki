# Using public_gemini

`public_gemini` folder is where you can place files to be hosted on your own Gemini subsection of `dimension.sh`. Any files placed in there will be available at the URL `gemini://dimension.sh/~yourusername/`.

The default page that'll be served if no filename is specified is `index.gmi`. Your `public_gemini` should already have an introductory file created for you as part of your new account. You can modify or remove this as needed. If no `index.gmi` is available for that folder, then the web server will generate a list of files.

## Writing .gmi Files

The full spec for Gemini Text can be found [here](https://gitlab.com/gemini-specification/gemini-text/-/blob/master/specification.gmi), but Flounder has a guide on [Writing gemtext](https://admin.flounder.online/gemini_text_guide.gmi). 

## Content Rules

We're not restrictive of what can be hosted in your `public_gemini` files; we ask that you keep within the [[Rules]]. From time to time, the admins will check the contents of any `public_gemini` folder to make sure everything is above board, and they will email if they have any issues.

## Helpful Tools

* [Awesome Gemini](https://github.com/kr1sp1n/awesome-gemini) - A full list of client, server, and other tools.
* [gemlog.sh](https://git.nytpu.com/gemlog.sh/about/) - A super simple gemlog tool.
* [Vulpes Proxy](https://proxy.vulpes.one/) - Minimalist Gopher/Gemini to HTTP proxy.