## Render deploy (static site)

This folder is a **self-contained static site** intended for deployment on Render.

### Contents
- `public/index.html`: the secure Thrive Summit deliverables page (client-side login).

### Important security note
The login credentials are embedded **client-side** inside `public/index.html` and will be visible to anyone who can view the page source. If you need real security, this must be served behind proper authentication (server-side) and the document should not be publicly accessible.

### Deploy to Render (via Git)
Render Static Sites deploy by cloning a Git repository.

Recommended settings when creating the Render Static Site:
- **Publish directory**: `public`
- **Build command**: `echo "no build"`

