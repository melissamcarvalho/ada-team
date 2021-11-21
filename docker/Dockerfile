FROM python:3.8

# Install Python libraries
COPY ./requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt

# Goes back to workspaces
WORKDIR "/workspaces"
