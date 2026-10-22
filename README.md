# Module 2 — instructor solutions

Worked versions of the seven labs of Module 2 (*Data Fusion, Preparation and Visualization
applied to Civil Engineering*), ACS-UPM Diploma in Engineering, Data Science and Artificial
Intelligence.

**This repository is private and must stay private.** The student material is public at
<https://github.com/antiafer/acs-upm-mod2-s01>; these are the answers to it.

```
solutions/
|-- Lab_1_1_reading_files_SOLUTION.ipynb              session 1
|-- Lab_1_2_object_and_field_SOLUTION.ipynb
|-- Lab_2_1_extraction_and_validation_SOLUTION.ipynb  session 2
|-- Lab_2_2_web_table_and_satellite_SOLUTION.ipynb
|-- Lab_3_1_json_SOLUTION.ipynb                       session 3
|-- Lab_3_2_api_pipeline_SOLUTION.ipynb
'-- Lab_3_3_web_scraping_SOLUTION.ipynb
```

## These files are generated: do not edit them here

Each lab has a single source, its notebook in `master/` of the course folder, where the answers
sit between `### BEGIN SOLUTION` and `### END SOLUTION`. `scripts/build_labs.py` turns that into
the student version, published in the public repository, and into the solution you see here.

Editing a file in this repository is lost on the next rebuild. Edit the master instead, rebuild,
and copy the result here.

## Running them

In Colab they work as they are: the setup cell finds no `data/` beside the notebook, so it clones
the public course repository into `/content` and reads the datasets from there.

Locally they need the course folder, because the setup cell looks for `data/` next to the notebook
or one level up. Run them from the `solutions/` folder of the course material, not from a clone of
this repository.

## State

All seven execute end to end, every `assert` passing. Session 3 reaches AEMET, Overpass and
Wikipedia: each call tries the network and falls back to a cached copy shipped in the public
repository, so no API key is needed and the labs work offline.
