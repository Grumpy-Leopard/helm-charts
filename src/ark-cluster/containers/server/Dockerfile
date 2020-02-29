FROM cm2network/steamcmd

WORKDIR /home/steam
USER steam

COPY --chown=steam:steam run-ark-server.sh ./run-ark-server.sh
RUN mkdir -p /home/steam/ark/ShooterGame/Saved/SavedArks \
    && chmod +x ./run-ark-server.sh


ENV MAP="TheIsland" \
    SESSIONNAME="Clustered Rancher-Based ARK Server on Kubernetes" \
    PORT="7777" \
    QUERYPORT="27015" \
    RCONPORT="32330" \
    SERVERADMINPASSWORD="YouShouldChangeThisWhenDeploying" \
    MAXPLAYERS="50" \
    CLUSTERID=""

VOLUME /home/steam/ark
VOLUME /home/steam/ark/ShooterGame/Saved

CMD ["./run-ark-server.sh"]
