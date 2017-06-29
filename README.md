# SOULITY/tvheadend-vaapi-kor
Tvheadend with VAAPI for KOREAN. \
This docker based on <lsiobase/alpine>, <linuxserver/docker-tvheadend>

Base-4.3/latest \
Tvheadend 4.3(Official) base. \
You must use ffmpeg pipe.

Base-4.1 \
Tvheadend 4.1(lekma custom+codec) base. \
You can use the VA-API codec profile in Tvheadend.
Also, can use ffmpeg pipe.

## Usage

```
docker create \
    --privileged \
    --name Tvheadend.VAAPI \
    --net=host \
    -v <Local config dir>:/home/tv/cfg \
    -v <Local recording dir>:/home/tv/rec \
    -e TZ="Asia/Seoul" \
    -e PUID="<root or user uid(ex. 1026)>" \
    -e PGID="<root or user gid(ex. 100)>" \
    -it soulity/tvheadend-vaapi-kor:<latest/Base-4.1p1/Base-4.3p1>
```

## Informations

## Versions
