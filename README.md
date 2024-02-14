# Servidor de Live Streaming com NGINX

Este projeto fornece um servidor simples para live streaming, implementado utilizando NGINX com suporte aos protocolos RTMP (Real Time Message Protocol) e HLS (HTTP Live Streaming). O objetivo é oferecer uma solução essencial para transmissão e visualização de streaming ao vivo.

## Desenvolvimento

Este projeto foi desenvolvido pela Lais Lima em seu canal do YouTube. O vídeo pode ser acessado [aqui](https://youtu.be/CrEzeBwLZPU).

## Requisitos

- [Docker](https://www.docker.com/)
- [Extensão para o Chrome "native MPEG-DASH + HLS Playback"](https://chromewebstore.google.com/detail/native-mpeg-dash-+-hls-pl/cjfbmleiaobegagekpmlhmaadepdeedn)
- [OBS](https://obsproject.com/pt-br/download)

## Tecnologias Utilizadas

- Docker Compose
- NGINX

## Protocolos Suportados

- RTMP (Real Time Message Protocol)
- HLS (HTTP Live Streaming)

## Como Executar

1. Suba os containers utilizando o Docker Compose:

    ```bash
    docker-compose up 
    ```

2. Abra o OBS e configure a transmissão, inserindo o seguinte servidor:

    ```
    rtmp://localhost:1935/live
    ```

    Clique em "OK" e, em seguida, clique em "Iniciar transmissão".

## Como Assistir à Transmissão

- No Chrome (com a extensão "MPEG-DASH + HLS Playback"), acesse:

    ```
    http://localhost:8081/live/.m3u8
    ```

## Recursos Adicionais

- Assista à [aula](https://youtu.be/CrEzeBwLZPU) relacionada ao desenvolvimento do projeto.
- Repositório original da criadora: [simple-live-streaming-server](https://github.com/lalizita/simple-live-streaming-server)
