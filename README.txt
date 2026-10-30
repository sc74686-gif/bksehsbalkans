BKSEHS MULTILINGUAL WEBSITE — VERSION 2

Included: English, Bosnian, Serbian, Albanian and Hebrew interface translations; responsive layout; separate Research, Interviews, News and Projects listing pages; article detail pages; Pages CMS configuration.

IMPORTANT ADMIN MODEL
The Admin link opens Pages CMS (https://app.pagescms.org/). Sign in with the GitHub account that owns the repository, install/authorize the Pages CMS GitHub App for the bksehsbalkans repository, then open that repository. The .pages.yml file configures editable content collections. Pages CMS is a separate hosted admin interface, not an embedded password form on the public site. It is free according to its official site/docs, but is a third-party service.

DEPLOYMENT
Upload the CONTENTS of this folder (not the ZIP itself) to the root of the GitHub repository. Then connect that GitHub repository to the existing Netlify site and set the publish directory to the repository root. For this plain HTML site, no build command is required. Do not delete the existing Netlify site.

CONTENT
Pages CMS manages JSON entries in content/research, content/interviews, content/news and content/projects. Add an item with a unique lowercase slug. The site list pages read index.json manifests; add the filename to the matching index.json after creating the item, or use the included GitHub editor to update the index.

LANGUAGES
The main interface supports en, bs, sr, sq, he. Each content type includes separate English, Bosnian, Serbian, Albanian and Hebrew title/summary/body fields. Add the translated text in the CMS; the site does not machine-translate content. A GitHub Actions workflow regenerates the listing indexes after content changes.

Contact: bksehs@outlook.com
