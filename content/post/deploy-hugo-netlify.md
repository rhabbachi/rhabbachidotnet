+++
title = "Deploy a Hugo static site on Netlify"
tags = ["Netfily", "Hugo", "Site", "Static Site", "Deploy"]
categories = ["How To's"]
draft = true
+++

# Why Netlify
- Price - free tire.
- Useful build configurations.
- Interesting extensions.

# Steps
- Connect
- Select repository.
- Add target repository.

When using a helper https://gohugo.io/content-management/formats/
Exemple rst2html
add requiremets.txt
check reference https://pip.pypa.io/en/stable/reference/pip_install/#requirement-specifiers

- Assets (Js/CSS) files not working
    make sure to build with `-b` (`--baseURL`).
- Better yet, Use a CDN.

# More
**Custom Domain**
https://docs.netlify.com/domains-https/custom-domains/#definitions


# References
- https://docs.netlify.com/
- https://gohugo.io/hosting-and-deployment/hosting-on-netlify/
- https://www.netlify.com/blog/2019/01/16/redirect-rules-for-all-how-to-configure-redirects-for-your-static-site/
