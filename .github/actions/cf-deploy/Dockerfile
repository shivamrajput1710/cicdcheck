FROM ppiper/cf-cli:v11

# needed for cf to find its config
# (GH resets HOME to /github/workspace)
ENV CF_HOME=$HOME
RUN chmod -R 777 .github/actions/cf-deploy/entrypoint.sh
# COPY entrypoint.sh /entrypoint.sh
ENTRYPOINT .github/actions/cf-deploy/entrypoint.sh
