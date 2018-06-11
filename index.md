---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

Ektelo is a programming framework and system that aids programmers in developing differentially private programs with high utility.  Ektelo can be used to author programs for a variety of statistical tasks that involve answering counting queries over a table of arbitrary dimension.

In Ektelo, a differentially private program is described as a *plan* over a high level library of *operators*.  Operators are organized into classes based on their functionality, which includes data transformations, data reductions, query selection and execution, and inference methods to combine noisy answers into a consistent estimate.
<!-- In addition, there are operators to partition the data so that it can be split or its dimensionality can be reduced.  The available operators are drawn from state-of-the-art algorithms in the published differential privacy literature. -->

The operator-based approach has following benefits:
- *Privacy for free*. Any plan written in Ektelo will satisfy differential privacy.  The privacy of each operator has been vetted and the system ensures that any composition of operators satisfies differential privacy.
- *Modularity*.  Ektelo enables code reuse as the same operator can be used in multiple programs.  This helps safety as the number of privacy-sensitive components is kept small.
- *Transparency*.  By expressing algorithms as plans with operators from operator classes, it is easier to compare/contrast competing algorithms.
<!-- - It also allows authors to easily modify algorithms. -->
- *Flexibility*.  Users can take existing operators and recombine them in arbitrary ways -- allowing them to invent new algorithms that borrow ideas from the state-of-art -- without the need for privacy analysis.

### Supporting publications

Dan Zhang, Ryan McKenna, Ios Kotsogiannis, Michael Hay, Ashwin Machanavajjhala, and Gerome Miklau. 2018. [EKTELO: A Framework for Defining Differentially-Private Computations](https://dl.acm.org/citation.cfm?id=3196921). In Proceedings of the 2018 International Conference on Management of Data ([SIGMOD '18](https://sigmod2018.org)). ACM, New York, NY, USA, 115-130. DOI: [https://doi.org/10.1145/3183713.3196921](https://doi.org/10.1145/3183713.3196921)

### Contributors

- [Dan Zhang](https://people.cs.umass.edu/~dzhang/), UMass Amherst
- [Ryan McKenna](https://people.cs.umass.edu/~rmckenna/), UMass Amherst
- [Ios Kotsogiannis](https://users.cs.duke.edu/~iosk/), Duke University
- [George Bissias](https://people.cs.umass.edu/~gbiss/), UMass Amherst
- [Michael Hay](cs.colgate.edu/~mhay/), Colgate University
- [Ashwin Machanavajjhala](http://users.cs.duke.edu/~ashwin/), Duke University
- [Gerome Miklau](http://people.cs.umass.edu/~miklau/index.html), UMass Amherst

### Acknowledgements

This project is supported by the NSF, DARPA and Center for Data Science at the University of Massachusetts College of Information and Computer Sciences.

<img src="{{ "/assets/logo-nsf.png" | absolute_url }}" height="75" width="75">
<img src="{{ "/assets/logo-darpa.jpg" | absolute_url }}" height="50">
<img src="{{ "/assets/logo-cds-cics.png" | absolute_url }}" height="45">
