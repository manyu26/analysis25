FROM rocker/rstudio:latest

# Install Python and Jupyter
RUN apt-get update && apt-get install -y python3 python3-pip && \
    pip3 install jupyterlab

# Install additional R packages
RUN Rscript -e 'install.packages(c("tidyverse", "igraph", "rmarkdown", "knitr"))'