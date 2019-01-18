FROM python:3-slim

LABEL version="0.0.1"
LABEL repository="http://github.com/ross/python-actions"
LABEL homepage="http://github.com/ross/python-actions"
LABEL maintainer="Ross McFarland <ross@github.com>"
LABEL com.github.actions.name="GitHub Action for PyTest"
LABEL com.github.actions.description="Action that allows for unit tests to be run using pytest"
LABEL com.github.actions.icon="package"
LABEL com.github.actions.color="blue"

COPY requirements.txt /requirements.txt
RUN pip install -r requirements.txt

COPY entrypoint.sh /entrypoint.sh

WORKDIR /workspace
ENTRYPOINT ["/entrypoint.sh"]
CMD ["--help"]
