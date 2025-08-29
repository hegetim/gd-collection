GD Collection v1
================

The *GD Collection v1* is a set of 4,890 graph drawings that we have extracted from 27
editions of the proceedings of the Symposium of Graph Drawing (and Network Visualization)
1998–2024.


Graph Storage Formats
---------------------

The collection contains graphs in [GEG]() (GEG Encodes Graphs) and GraphViz dot file formats.
Note that while widely used, the dot format extensions for edge geometries (as defined in Appendix F
of their [User's Manual](https://graphviz.org/pdf/dotguide.pdf)) is rather niche and may not be
supported by most software.  We recommend using the GEG versions.


Metadata
--------

Each GEG/dot file contains a mandatory set of metadata.  Directedness which is always `false` due to
limitations of our pipeline even if the original drawing was directed, the digital object identifier
(DOI) of the publication, and the figure number if our tools were able to extract it (note that this
was not very reliable).

Refer to `gd_metadata.csv` in the root directory of this repository for title, pages, and authors.


Harvesting Graphs
-----------------

The drawings were extracted in a fully automated and unsupervised process using
[Graph Harvester](https://github.com/hegetim/graph-harvester-v2).
Note that Graph Harvester can only handle vector graphics.  In a first evaluation, where we manually
checked 101 articles picked at random, we found that Graph Harvester managed to extract 48% of all
graph drawings in the PDFs and of these 69% were of high quality (i.e. they accurately reproduce the
adjacencies and edge paths depicted).


Publication
-----------

If you find our work useful for your research, consider citing our paper:

```bibtex
@InProceedings{mhwwp-uqm-GD25,
  author =    {Mooney, Gavin and Hegemann, Tim and and Wolff, Alexander and Wybrow, Michael and Purchase, Helen},
  title =     {Universal Quality Metrics for Graph Drawings: Which Graphs Excite Us Most?},
  booktitle = {Graph Drawing and Network Visualization (GD)},
  year =      {2025},
  series =    {LIPIcs},
  volume =    357,
  editor =    {Dujmovi{\'c}, Vida and Montecchiani, Fabrizio},
  publisher = {Schloss Dagstuhl~-- Leibniz-Zentrum f{\"u}r Informatik},
}
```


Contributors
------------

This collection is joint work by the
[algorithms and complexity group](https://www.informatik.uni-wuerzburg.de/algo/team/),
University of Würzburg, Germany
and the [embodied visualisation group](https://www.monash.edu/it/hcc/embodied-visualisation),
Monash University, Australia.

For contact, you can write an email to ``hegemann *at* informatik *dot* uni-wuerzburg *dot* de``.

