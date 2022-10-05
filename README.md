# SPSRC User Docs

User documentation for the SKA Regional Centre prototype at the IAA-CSIC. 

[![Documentation Status](https://readthedocs.org/projects/spsrc-user-docs/badge/?version=latest)](https://spsrc-user-docs.readthedocs.io/en/latest/?badge=latest)

<HR>

# Deploy live documentation in your own computer with `docker`

- Clone this repository: ``git clone <this repository>``
- Go to the folder ``cd spsrc_user_docs``
- Run the following command: ``docker run --rm -it -p 18022:8000 -v ${PWD}:/docs squidfunk/mkdocs-material``
- Go to your browser http://localhost:18022 


