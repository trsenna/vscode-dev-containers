FROM trsenna/vscodedevimages-foundation:base

# ENV DEBIAN_FRONTEND=noninteractive

# RUN sudo apt-get -y update --no-install-recommends \
#     && sudo apt-get -y install --no-install-recommends \
#     <your-package-list-here> \
#     && sudo apt-get autoremove -y \
#     && sudo apt-get clean -y

RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \
    && sudo bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/miniconda \
    && sudo chown -R vscode:vscode /opt/miniconda \
    && /opt/miniconda/bin/conda init bash

ENV PATH=$PATH:/opt/miniconda/pcondabin:/opt/miniconda/bin
