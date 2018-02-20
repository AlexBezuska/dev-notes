# .htaccess

name the file `.htaccess`


## Redirects


### 301 (Permanent) Redirect 
Point an entire site to a different URL on a permanent basis. 
This is the most common type of redirect and is useful in most situations. In this example, we are redirecting to the "mt-example.com" domain:

`Redirect 301 / http://mt-example.com/`

### 302 (Temporary) Redirect
Point an entire site to a different temporary URL. 
This is useful for SEO purposes when you have a temporary landing page and plan to switch back to your main landing page at a later date:

`Redirect 302 / http://mt-example.com/`

### Redirect index.html to a specific subfolder:
This allows you to redirect index.html to a specific subfolder

`Redirect /index.html http://example.com/newdirectory/`

### Redirect old file path to new file path

`Redirect /olddirectory/oldfile.html http://example.com/newdirectory/newfile.html`

### Redirect to a specific index page:
Provide Specific Index Page (Set the default handler)

`DirectoryIndex index.html`
