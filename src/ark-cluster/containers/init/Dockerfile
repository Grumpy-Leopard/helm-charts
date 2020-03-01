FROM cm2network/steamcmd

LABEL maintainer="support@grumpyleopard.com"

WORKDIR /home/steam
USER steam

RUN mkdir -p mkdir -p /home/steam/ark/ShooterGame/Saved/SavedArks

VOLUME /home/steam/ark

CMD ["./steamcmd/steamcmd.sh","+login","anonymous","+force_install_dir","/home/steam/ark","+app_update","376030","validate","+quit"]
