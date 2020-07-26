Citation
========

If you make use of ePSdata results in your research, please cite as follows. (`Get the citations as a .bib file here. <_files/cite_ePSdata.bib>`_)

Dataset
-------
Each ePSdata webpage corresponds to a dataset, with a unique DOI, and citation details at the foot of the page. Each webpage originates as a Jupyter Notebook, which employs `ePSproc <https://epsproc.readthedocs.io>`_ to process and visualise an `ePolyScat <http://www.chem.tamu.edu/rgroup/lucchese/>`_ dataset; these all share the DOI, and are packaged together and uploaded to a `Zenodo <https://zenodo.org>`_ repository. (Zenodo is hosted by CERN, and follows `Open Science <https://about.zenodo.org>`_ and `FAIR principles <https://about.zenodo.org/principles/>`_.)

These have the general form, following [DataCite]_, in Bibtex format::

  @data{datasetName,
    title = {ePSproc: datasetName}
    author = {Hockett, Paul},
    doi = {...},
    publisher = {Zenodo},
    year = {...},
    url = {https://phockett.github.io/ePSdata/...}
  }

(Note that @data may not be supported in all cases, use @misc instead - see, for instance, `this discussion on duecredit/Zenodo bibtex entries <https://github.com/duecredit/duecredit/issues/77>`_. Another viable route is reformatting as `@article` with "Dataset on Zenodo" for the journal name, see `Publishing Datasets on Zenodo and Citing them with Mendeley for discussion <https://allixender.blogspot.com/2018/02/publishing-datasets-on-zenodo-and.html>`_. For other citation styles/options, try putting a specific DOI into `citation.crosscite.org <https://citation.crosscite.org>`_.)


Computational tools
-------------------

The results here use `Gamess <http://www.msg.ameslab.gov/gamess/>`_, `ePolyScat <http://www.chem.tamu.edu/rgroup/lucchese/>`_ and `ePSproc <https://epsproc.readthedocs.io>`_. See the `methods` page for details.

For `Gamess <http://www.msg.ameslab.gov/gamess/>`_::

  @article{Gamess1993,
    author = {Schmidt, Michael W and Baldridge, Kim K and Boatz, Jerry A and Elbert, Steven T and Gordon, Mark S and Jensen, Jan H and Koseki, Shiro and Matsunaga, Nikita and Nguyen, Kiet A and Su, Shujun and Windus, Theresa L and Dupuis, Michel and Montgomery, John A},
    doi = {10.1002/jcc.540141112},
    issn = {1096-987X},
    journal = {Journal of Computational Chemistry},
    number = {11},
    pages = {1347--1363},
    publisher = {John Wiley {\&} Sons, Inc.},
    title = {{General atomic and molecular electronic structure system}},
    url = {http://dx.doi.org/10.1002/jcc.540141112},
    volume = {14},
    year = {1993}
  }
  @incollection{Gamess2005,
    author = {Gordon, Mark S. and Schmidt, Michael W.},
    booktitle = {Theory and Applications of Computational Chemistry},
    chapter = {41},
    doi = {10.1016/B978-044451719-7/50084-6},
    pages = {1167--1189},
    publisher = {Elsevier},
    title = {{Advances in electronic structure theory}},
    url = {https://linkinghub.elsevier.com/retrieve/pii/B9780444517197500846},
    year = {2005}
  }
  @misc{GamessWebsite,
    author = {Gordon, Mark S.},
    title = {{Gamess website}},
    url = {http://www.msg.ameslab.gov/gamess/}
  }


For `ePolyScat <http://www.chem.tamu.edu/rgroup/lucchese/>`_::

  @article{ePS1994,
    author = {Gianturco, F. A. and Lucchese, R. R. and Sanna, N.},
    doi = {10.1063/1.467237},
    issn = {00219606},
    journal = {The Journal of Chemical Physics},
    month = {may},
    number = {9},
    pages = {6464},
    publisher = {AIP Publishing},
    title = {{Calculation of low-energy elastic cross sections for electron-CF4 scattering}},
    url = {http://scitation.aip.org/content/aip/journal/jcp/100/9/10.1063/1.467237},
    volume = {100},
    year = {1994}
  }

  @article{ePS1999,
    author = {Natalense, Alexandra P P and Lucchese, Robert R},
    doi = {10.1063/1.479794},
    issn = {00219606},
    journal = {The Journal of Chemical Physics},
    number = {12},
    pages = {5344},
    title = {{Cross section and asymmetry parameter calculation for sulfur 1s photoionization of SF[sub 6]}},
    url = {http://link.aip.org/link/JCPSA6/v111/i12/p5344/s1{\&}Agg=doi},
    volume = {111},
    year = {1999}
  }

  @misc{ePSWebsite,
    author = {Lucchese, R. R.},
    title = {{Lucchese Group Website}},
    url = {http://www.chem.tamu.edu/rgroup/lucchese/},
  }


For `ePSproc <https://epsproc.readthedocs.io>`_:

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


.. [DataCite] Fenner, M. et. al. (2019). A data citation roadmap for scholarly data repositories. Scientific Data, 6(1), 28. `DOI: 10.1038/s41597-019-0031-8 <https://doi.org/10.1038/s41597-019-0031-8>`_
