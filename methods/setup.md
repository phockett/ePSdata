Refs

- [GH pages docs](https://help.github.com/en/github/working-with-github-pages)
- [Publishing Sphinx docs on Github pages](https://soderstrom-rikard.github.io/git/publishing-sphinx-generated-docs-on-github-pages.html)
- [Publishing from Sphinx (this one keeps the source separate)](https://daler.github.io/sphinxdoc-test/includeme.html)
- [nojekyll Sphinx extension](https://www.sphinx-doc.org/en/master/usage/extensions/githubpages.html#module-sphinx.ext.githubpages)

[Basically just need `docs` on master branch, or set `gh-pages` branch with docs.](https://help.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#choosing-a-publishing-source)

Can also use [submodules to bring in content from other projects](https://help.github.com/en/github/working-with-github-pages/using-submodules-with-github-pages).


10/01/20
Setting up on Bemo. Mainly following simple guide: [Publishing Sphinx docs on Github pages](https://soderstrom-rikard.github.io/git/publishing-sphinx-generated-docs-on-github-pages.html)

- New repo on Github, ePSdata.
- Clone to ~/python/ePSdata

- Make gh-pages branch
git checkout --orphan gh-pages
git commit
git push --set-upstream origin gh-pages


- Add master as submodule... doesn't work, gives
git remote add https://github.com/phockett/ePSdata build/html


- Setup Sphinx
sphinx-quickstart

Add nbsphinx extension to conf.py.

- HTML conversion
