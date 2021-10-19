---
layout: post
author: kalju
---

Maybe I'm expecting too much, but I spent the morning chasing down a url bug. The GitHub Pages site adds the repo name to the url, breaking the <a href="https://jekyllrb.com/docs/step-by-step/08-blogging/">jekyll blog tutorial</a> navigation.  
It gets explained in more detail <a href="https://github.com/jekyll/jekyll/issues/332">here</a>. This link is ten years old, but as far as I can tell contains the most viable solution.
Adding a prefix to every url instance feels wrong, and makes me want to create a reusable component that adds the prefix. But then if I'm doing that, should I just be using React? I was expecting Jekyll to handle 'this sort of thing' for me.

I ended up biting the bullet and adding in the url prefixes. Now that I've done it, the experience wasn't as bad as I expected. But I'll remember this, Jekyll.

rejected solutions:

I considered using Docusaurus for this blog, as I plan on using it for the <a href="www.nice-train.com">Nice Train</a> design documentation. It has a <a href="https://docusaurus.io/docs/deployment#deploying-to-github-pages">guide for GitHub Pages hosting</a>, and looks like it addresses this specific issue. However, the configuration looks complex enough that I rolled back into using Jekyll (for now).

An <a href="https://github.com/jekyll/jekyll/issues/332#issuecomment-1166721">obtuse comment</a> suggested using a \<base> tag. I noticed this after I already implemented the 'baseurl' solution, and it looks like it <a href="https://stackoverflow.com/questions/11521011/why-base-tag-does-not-work-for-relative-paths">might come with its own fiddlyness</a>. Maybe I'll revisit this solution if this blog structure grows to the point that the current solution is a pain to maintain.
