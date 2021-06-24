# Using public_html

`public_html` folder is where you can place files to be hosted on your own subsection of `dimension.sh`. Any files placed in there will be available at the URL `https://dimension.sh/~yourusername/`.

The default page that'll be served if no filename is specified is `index.html`. Your `public_html` should already have an introductory file created for you as part of your new account. You can modify or remove this as needed. If no `index.html` is available for that folder, then the web server will generate a list of files.

## Content Rules

We're not restrictive of what can be hosted in your `public_html` files; we ask that you keep within the [[Rules]]. From time to time, the admins will check the contents of any `public_html` folder to make sure everything is above board, and they will email if they have any issues.

## What is supported?

* Basic [SSI](http://nginx.org/en/docs/http/ngx_http_ssi_module.html#commands) (Server Side Includes).
* Custom 404 pages (name the file `404.html` in your `public_html`)
* Custom 50x pages (name the file `500.html` in your `public_html`)

## What we _don't_ support at the moment

* CGI scripts - ([In progress](https://github.com/dimension-sh/infra/issues/11))
* PHP

## Helpful Tools

We have the following tools installed on `dimension.sh` to help you make your own site.

* [Hugo](https://gohugo.io) - A static site generator 