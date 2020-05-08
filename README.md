coronamaze.org
==============

This repo is the public pages site for www.coronamaze.org

CoronaMaze is aimed to be a website to help the kids arond the world with the confinement due to the coronavirus, proposing all the kids a new challenge every day to help them keep their mind awake in a happy way during those hard times.

I am doing this with Jekyll for the automation of the creation of the static site. I'm still unsure of the final URL schema and also how the data will be structured. If you want to collaborate, contact me at xavi.coronamaze@gmail.com before forking or doing PRs.

The reason for publishing without having this for clear is to minimize the time to get published so the kids around the world can start to have fun without more delay in this new coronavirus epoch.

Tech stack
----------

* The source code is hosted at https://github.com/xmontero/coronamaze-static-web
* Uses https://jekyllrb.com/ for templating and building. The reason behind is that Github Pages is using that engine.
* The pages are hosted by GitHub Pages under the custom domain www.coronamaze.org
 
To help devel
-------------

You need jekyll.

From your docker host:

    docker run -it --rm -p 4000:4000 -v /your/project/directory:/files --name jekyll --hostname jekyll -u ubuntu jekyll bash

From the inside of the docker (the first time you run the image):

    cd /files
    bundle install
    bundle exec jekyll serve --force_polling -H 0.0.0.0 -P 4000

If you don't use the `--rm` tag and re-use a jekyll machine, skip the `bundle install` from the second time on:

    cd /files
    bundle exec jekyll serve --force_polling -H 0.0.0.0 -P 4000
 
 Help needed
 -----------
 
 - Translators (native, if possible)
 - Localization managers
 - Localization engineers
 - Frontend engineers
  
 Contact
 -------
 
 xavi.coronamaze@gmail.com
 