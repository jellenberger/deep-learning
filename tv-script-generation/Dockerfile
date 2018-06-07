# Start from a core stack version
FROM jupyter/tensorflow-notebook

# Switch to root user
USER root

# # Install debian packages
# RUN apt-get update && apt-get -y upgrade \
#     && apt-get -y install \
#         postgresql-client \
#         curl \
#     && apt-get clean && apt-get autoremove \
#     && rm -rf /var/lib/apt/lists/*

# Switch to the non-root user
USER $NB_UID

# # Install some conda data science and ml stuff
# RUN conda update -n base conda \
#     && conda install -y \
#         pyyaml h5py \
#         opencv \
#     && conda clean -tipsy

# # Install some misc pip packages
# RUN pip install --user psycopg2-binary

# Start in work directory
WORKDIR $HOME/work