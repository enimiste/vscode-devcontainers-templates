FROM mcr.microsoft.com/devcontainers/base:jammy

USER vscode

RUN curl -s "https://get.sdkman.io" | bash
RUN chmod +x "$HOME/.sdkman/bin/sdkman-init.sh"
RUN "$HOME/.sdkman/bin/sdkman-init.sh"


# Java Env
RUN zsh -c "source $HOME/.sdkman/bin/sdkman-init.sh && sdk install java 17.0.9-tem"

#Scala Env
RUN zsh -c "source $HOME/.sdkman/bin/sdkman-init.sh && sdk install sbt && sdk install scala && sdk install scalacli"
