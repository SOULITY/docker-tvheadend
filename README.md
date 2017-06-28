Tvheadend with VAAPI for KOREAN. \
This docker based on <lsiobase/alpine>, <linuxserver/docker-tvheadend>

Base-4.3(latest) \
Tvheadend 4.3(Official) base. \
Base-4.1 \
Tvheadend 4.1(lekma custom) base.

USE: \
docker create \
    --privileged \
    --name Tvheadend.VAAPI \
    --net=host \
    -v <Local config dir>:/home/tv/cfg \
    -v <Local recording dir>:/home/tv/rec \
    -e TZ="Asia/Seoul" \
    -e PUID="<root or user uid(ex. 1026)>" \
    -e PGID="<root or user gid(ex. 100)>" \
    -it soulity/tvheadend-vaapi-kor
