# Home Server Docker Configurations

This repository contains configuration files for managing Docker services on my private home server.

> Each service is organized in its own directory with a corresponding `docker-compose.yaml` or `docker-compose.yml` file for easy deployment and management.

## Services

- [**Duck DNS**](https://hub.docker.com/r/linuxserver/duckdns): Dynamic DNS service using DuckDNS.
- [**FlareSolverr**](https://github.com/FlareSolverr/FlareSolverr): Proxy server to bypass Cloudflare protection.
- [**Home Assistant**](https://www.home-assistant.io/installation/linux#docker-compose): Home automation platform running via Docker.
- [**Jellyfin**](https://jellyfin.org/docs/general/installation/container#docker): Media server for streaming movies, TV shows, and music.
- [**Jenkins**](https://www.jenkins.io/doc/book/installing/docker/): Automation server for CI/CD pipelines.
- [**Paperless-ngx**](https://docs.paperless-ngx.com/setup/#docker): Document management system.
- [**Pi-hole**](https://github.com/pi-hole/docker-pi-hole): Network-wide ad blocker.
- [**Portainer**](https://docs.portainer.io/start/install/server/docker/linux): Docker management UI.
- [**Prowlarr**](https://wiki.servarr.com/prowlarr/installation/docker): Indexer manager/proxy for various media applications.
- [**Radarr**](https://wiki.servarr.com/radarr/installation/docker): Movie collection manager for Usenet and BitTorrent users.
- [**Reiverr**](https://github.com/reiverr/reiverr): Combined interface for Jellyfin, TMDB, Radarr and Sonarr.
- [**Sonarr**](https://wiki.servarr.com/sonarr/installation/docker): TV series collection manager for Usenet and BitTorrent users.
- [**Teleport**](https://goteleport.com/docs/installation/#docker): Secure access to infrastructure.
- [**Traefik**](https://doc.traefik.io/traefik/getting-started/install-traefik/#use-the-official-docker-image): Reverse proxy and load balancer.
- [**Transmission**](https://hub.docker.com/r/linuxserver/transmission): BitTorrent client.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone <this-repo-url>
   cd aorus
   ```
2. **Configure environment variables:**

   - Edit the relevant `docker-compose.yaml`/`.yml` files and any config files as needed for your environment.

3. **Start a service:**

   ```bash
   cd <service-directory>
   docker compose up -d # To specify a custom environment file, use the `--env-file` option
   ```

4. **Stop a service:**
   ```bash
   docker compose down
   ```

## License

This repository is for personal use. Please review each service's license before deploying in a production environment.
