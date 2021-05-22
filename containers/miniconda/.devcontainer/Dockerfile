FROM trsenna/vscodedevimages-foundation:base

# ENV DEBIAN_FRONTEND=noninteractive

# RUN apt-get -y update --no-install-recommends \
#     && apt-get -y install --no-install-recommends \
#     <your-package-list-here> \
#     && apt-get autoremove -y \
#     && apt-get clean -y

RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \
    && bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/miniconda \
    && chown -R vscode:vscode /opt/miniconda \
    && /opt/miniconda/bin/conda init bash

ENV PATH=$PATH:/opt/miniconda/pcondabin:/opt/miniconda/bin
