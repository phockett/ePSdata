Citation
========

If you make use of ePS data results in your research, please cite as follows.

Dataset
-------
Each ePSdata page corresponds to a dataset, with a unique DOI, and citation details at the foot of the page.

These have the general form:




Computational tools
-------------------

The results here use Gamess, ePolyScat and ePSproc. See the `methods` page for details.

For Gamess:



For ePolyScat:



For ePSproc:

Cite the software directly via either Github or Figshare repositories for the software (note same DOI for both)::

  @misc{ePSprocGithub,
    title={ePSproc: Post-processing for ePolyScat},
    url={https://github.com/phockett/ePSproc},
    DOI={10.6084/m9.figshare.3545639},
    publisher={Github},
    howpublished = {\url{https://github.com/phockett/ePSproc}},
    author={Hockett, Paul},
    year={2016},
    commit = {30158eb3fbba41d0a4c3a973744f28b7187e6ee2}
  }

  @misc{ePSprocFigshare,
    title={ePSproc: Post-processing for ePolyScat},
    url={https://figshare.com/articles/ePSproc_Post-processing_for_ePolyScat_v1_0_0_/3545639/4},
    DOI={10.6084/m9.figshare.3545639},
    publisher={Figshare},
    author={Hockett, Paul},
    year={2016}
  }

... or the software paper (Authorea/arXiv)::

  @article{ePSprocPaper,
    title={ePSproc: Post-processing for ePolyScat electron-molecule scattering calculations},
    url={https://www.authorea.com/users/71114/articles/122402-epsproc-post-processing-suite-for-epolyscat-electron-molecule-scattering-calculations},
    DOI={10.22541/au.156754490.06103020},
    journal = {Authorea/arXiv e-prints},
    publisher={Authorea/arXiv},
    author={Hockett, Paul},
    year={2016},
    archivePrefix = {arXiv},
    eprint = {1611.04043},
    primaryClass = {physics.comp-ph},
    eid = {arXiv:1611.04043},
    pages = {arXiv:1611.04043}
  }

(Citation styles for software `from StackExchange <https://academia.stackexchange.com/questions/14010/how-do-you-cite-a-github-repository>`_.)

.. .. include:: citation.txt (keep duplicate details here, since this doesn't work for basic Github readme!)

Acknowledgements
----------------

Special thanks to R.R. Lucchese and coworkers for `ePolyScat <http://www.chem.tamu.edu/rgroup/lucchese/ePolyScat.E3.manual/manual.html>`_.

Thanks, finally, and of course, to those supporting scientific software development and infrastructure (and making it easy!), including Github, Read the Docs, Pypi, SciPy etc. etc. In particular the python version of ePSproc makes use of `Xarray <http://xarray.pydata.org/en/stable/index.html>`_, and `Moble's spherical functions (& quaternion) <https://github.com/moble/spherical_functions>`_. See `methods` for more details.
