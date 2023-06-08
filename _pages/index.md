---
layout: home
author_profile: true
permalink: /
title: Welcome!

# Delete next lines if you prefer not to have a feature row
feature_row_title: Academic Interests
feature_row:
  - image_path: /images/p1.jpg
    alt: "iDEA"
    title: "Academic interest 1"
    excerpt:
        "This is a description of item 1"
  - image_path: /images/p1.jpg
    alt: "Academic interest 2"
    title: "Academic interest 2"
    excerpt:
        "This is a description of item 2"
  - image_path: /images/p1.jpg
    alt: "Academic interest 3"
    title: "Academic interest 3"
    excerpt:
        "This is a description of item 3"
# Delete the previous lines if you prefer not to have a feature row
---
<p style="text-align: justify">
I am a Ph.D. candidate in the Department of Biostatistics at the University of Michigan, Ann Arbor. I have been working with <a href="https://www.xzlab.org">Dr. Xiang Zhou</a> on developing statistical and computational methods for genomics and genetics data. My recent research interests focus on developing efficient statistical learning methods to address a variety of biological problems and computational challenges in genomics and genetics, particularly single-cell RNA-sequencing, and spatially resolved transcriptomics. In addition to my methodological research, I also work on genetic risk prediction analysis for common health exposure traits in large biobanks such as UK Biobank, and the <a href="https://precisionhealth.umich.edu/our-research/michigangenomics/">Michigan Genomics Initiative (MGI)</a>. I will be joining as an Assistant Professor at the <a href="https://www.brown.edu/academics/public-health/biostats/home">Department of Biostatistics</a> and as a member at the <a href="https://ccmb.brown.edu">Center for Computational Molecular Biology</a> at Brown University this summer.
</p>

<!-- Delete next line if you prefer not to have a feature row. -->
<br />
<br />
{% if page.feature_row %}
  {% include feature_row %}
{% endif %}
<!-- Delete previous lines if you prefer not to have a feature row. -->
