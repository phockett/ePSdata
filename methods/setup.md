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

This works:
git remote add html https://github.com/phockett/ePSdata/build/html
... but not sure that's the intention.
>>> Pages served OK from https://phockett.github.io/ePSdata/build/html/index.html
May just need to add html redirect in project root.
Could also just change docs dir, e.g. as per https://daler.github.io/sphinxdoc-test/includeme.html


- Setup Sphinx
sphinx-quickstart

Add nbsphinx extension to conf.py
(plus settings - adapted from NBsphinx example docs:
  #	https://nbsphinx.readthedocs.io/en/0.4.3/prolog-and-epilog.html
  #	https://nbsphinx.readthedocs.io/en/0.4.3/conf.py
  )

- Dir structure
  -- build
  -- source  
    - index.rst
    -- mol dirs with .ipynb docs.

- Set index.rst with epsman/web/buildSphinxHTML.genSphinxIndex()
Pulls in subdirs as sepearte toctrees.

- HTML build (Bemo)
conda activate webDev
make html

16/01/20
Fixing structure... want root pages at https://phockett.github.io/ePSdata/
NOT https://phockett.github.io/ePSdata/build/html/ as currently.

Issue with file structure... easiest to:
(A) dump everything back to master branch.
(B) include only HTML/ on gh-pages?  (Or docs on master?)

Currently can't merge branches, as they are totally different...

GIT FOR GITHUB PAGES

Copy file foo between branches
https://stackoverflow.com/questions/17416691/how-can-i-copy-files-from-a-branch-to-another-using-git
git checkout gh-pages
git checkout master foo
git commit -m 'Add file foo to gh-pages.'

From a specific commit
https://stackoverflow.com/questions/307579/how-do-i-copy-a-version-of-a-single-file-from-one-git-branch-to-another#307872
git checkout <commit_hash> <relative_path_to_file_or_dir>
git checkout <remote_name>/<branch_name> <file_or_dir>

For a dir:
https://stackoverflow.com/questions/307579/how-do-i-copy-a-version-of-a-single-file-from-one-git-branch-to-another#307872
git checkout other-branch app/**
