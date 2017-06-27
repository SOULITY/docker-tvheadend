Tvheadend with VAAPI(ffmpeg) for KOREAN.
This docker based on <lsiobase/alpine> & <linuxserver/docker-tvheadend>

USE:

docker create \
    --privileged \
    --name Tvheadend.VAAPI \
    --net=host \
    -v /dev/dri:/dev/dri \
    -v <Local config dir>:/home/tv/cfg \
    -v <Local recording dir>:/home/tv/rec \
    -e TZ="Asia/Seoul" \
    -e PUID="<root or user uid(ex. 1026)>" \
    -e PGID="<root or user gid(ex. 100)>" \
    -it soulity/tvheadend-vaapi-kor
