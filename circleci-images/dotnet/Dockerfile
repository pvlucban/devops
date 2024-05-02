FROM cimg/base:stable

# Install .NET SDK 8
RUN sudo apt-get update && \
    sudo apt-get install -y apt-transport-https && \
    sudo apt-get update

RUN wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb && \
    sudo dpkg -i packages-microsoft-prod.deb && \
    sudo rm packages-microsoft-prod.deb

RUN sudo apt-get update && \
    sudo apt-get install -y dotnet-sdk-8.0

RUN sudo apt-get install ca-certificates libc6 libgcc-s1 libgssapi-krb5-2 libicu66 libssl1.1 libstdc++6 zlib1g
RUN sudo apt-get update