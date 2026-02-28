FROM mcr.microsoft.com/devcontainers/base:trixie

RUN curl -SLO $(curl -s https://api.github.com/repos/Vanilla-OS/Vib/releases/latest | jq -r '.assets.[] | select(.name == "vib-amd64") | .browser_download_url') \
 && sudo mv vib-amd64 /usr/bin/vib \
 && sudo chmod +x /usr/bin/vib

RUN curl -SLO $(curl -s https://api.github.com/repos/Vanilla-OS/Vib/releases/latest | jq -r '.assets.[] | select(.name == "plugins-amd64.tar.gz") | .browser_download_url') \
 && sudo mkdir -p /usr/share/vib/plugins \
 && sudo tar -xvf plugins-amd64.tar.gz -C /usr/share/vib/plugins/ --strip-components=2

RUN curl -SLO $(curl -s https://api.github.com/repos/Vanilla-OS/vib-fsguard/releases/latest | jq -r '.assets.[] | select(.name == "fsguard-amd64.so") | .browser_download_url') \
 && sudo mv fsguard-amd64.so /usr/share/vib/plugins/fsguard.so
