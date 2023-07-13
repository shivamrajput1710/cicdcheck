FROM ppiper/cf-cli:v11

# needed for cf to find its config
# (GH resets HOME to /github/workspace)
ENV CF_HOME=$HOME
RUN chmod +x /entrypoint.sh
COPY entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]