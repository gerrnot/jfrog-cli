FROM releases-docker.jfrog.io/jfrog-ecosystem-integration-env:latest
ARG image_name=jfrog-cli-full
ARG cli_executable_name=jf
COPY ${cli_executable_name} /usr/local/bin/${cli_executable_name}
RUN chmod +x /usr/local/bin/${cli_executable_name}
# Install bash completion
RUN ${cli_executable_name} completion bash >> /etc/bash_completion
