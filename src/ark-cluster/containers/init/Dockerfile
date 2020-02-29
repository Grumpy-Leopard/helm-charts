FROM cm2network/steamcmd

WORKDIR /home/steam
USER steam

VOLUME /home/steam/ark

CMD ["./steamcmd/steamcmd.sh","+login","anonymous","+force_install_dir","/home/steam/ark","+app_update","376030","validate","+quit"]
