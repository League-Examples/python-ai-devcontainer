FROM ghcr.io/league-examples/python-devcontainer:latest

LABEL org.opencontainers.image.description DESCRIPTION="Microsoft Python 3.12 Dev Container, tailored for League AI projects"

ARG VNC_RESOLUTION=600x600x16


# copy requirements list into layer of dev image
COPY requirements.txt /workspaces/session/requirements-ai.txt
RUN python -m pip install --upgrade pip
RUN pip --disable-pip-version-check --no-cache-dir install -r /workspaces/session/requirements-ai.txt

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update \
#     && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>
