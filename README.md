# Best Practices for Releasing Experiment Artifacts

## Introduction

The intent of this document is to provide some recommendations for releasing experiment artifacts to aid the research community.

## Templates

As an attempt to put discussion into action, the templates directory contains a base README.md template that will aid the discovery and ingestion of experimental artifacts.

Please check the [README.md template](templates/README.md) for your artifact repositories.

## Best Practice Recommendations

### 1. Specification of Dependencies

Any pre-requisite dependencies that your experiment has should be listed to help aid in the reproducibility of your experiment. Following are some recommendations to consider :

1. You should likely assume little if any background on the technology that your artifact relies on to best increase the likelihood of re-use.
2. Attempt to be clear and concise with your instructions to make sure that entities looking to re-use your artifacts can do so without your assistance.
3. If feasible, try to provide an entirely re-producible version of your artifact by leveraging systems such as docker to provide a docker image in Dockerhub and Dockerfile for re-creation.

### 2. Artifacts

The artifacts that you want to share should be included in the form that they are most useful in. Consider items like the following as you share them with other researchers:

1. Completeness of the artifacts. Make sure to include everything that is necessary for your experiment validation.
2. It is most useful if artifacts are shared in a common or well-known format to aid in other research re-use. While proprietary formats may sometimes be required, any tools that aid that access to that data should be pointed out to lower the learning curve for potential use.

#### Types of Artifacts

Consider including artifacts like the following :

1. Datasets
2. Code
3. Configurations
4. Experiment setup tools
5. System images (e.g., docker images)
6. Testbed specific initiation scripts
7. Publications related to this artifact

### 3. Evaluation Code

Experiments may have subtleties that were not possible to explain in the research paper due to space constraints. Including the code you used for setup, collection, reformatting, or analysis along with a description of what that code is and where it is used in the experimental pipeline can be extremely helpful to your fellow researchers.

### 4. Other Items to Consider

If you are using specific scientific disciplines for your work, it may be useful to include additional items. For example:

1. For ML-based efforts, consider checking out the ML recommendations [here](https://github.com/paperswithcode/releasing-research-code).

### 5. Specific Results

If can be useful to provide some of your key results as part of the sharing of your artifacts. Consider including a table of those results, graphs showing those results, along with the specific commands utilized to generate those results from the shared artifacts.

## Useful Resources

These recommendations come from the ML recommendations mentioned above. Modified to suit the needs of this document.

### Hosting Files

1. [Zenodo](https://zenodo.org) - versioning, 50GB, free bandwidth, DOI, provides long-term preservation
2. [GitHub Releases](https://help.github.com/en/github/administering-a-repository/managing-releases-in-a-repository) - versioning, 2GB file limit, free bandwidth
3. [OneDrive](https://www.onedrive.com/) - versioning, 2GB (free)/ 1TB (with Office 365), free bandwidth
4. [Google Drive](https://drive.google.com) - versioning, 15GB, free bandwidth
5. [Dropbox](https://dropbox.com) - versioning, 2GB (paid unlimited), free bandwidth
6. [AWS S3](https://aws.amazon.com/s3/) - versioning, paid only, paid bandwidth
7. [DAGsHub](https://dagshub.com) - a way to track experiments, version data, models & pipelines, using Git

### Managing Files

1. [RClone](https://rclone.org/) - provides unified access to many different cloud storage providers
2. [dvc](https://dvc.org) - open-source version control system designed for machine learning projects

### Making Project Pages

1. [GitHub pages](https://pages.github.com/)
2. [Fastpages](https://github.com/fastai/fastpages)

### Making Demos and Tutorials

1. [Google Colab](https://colab.research.google.com/)
2. [Binder](https://mybinder.org/)
3. [Streamlit](https://github.com/streamlit/streamlit)

## Contributing

If you'd like to contribute to these best practices please open an issue on this GitHub repository or submit a pull request. Also, please check out the NSF SEARCCH [project](https://searcch.cyberexperimentation.org).

All content in this repository is licensed under the MIT license.
