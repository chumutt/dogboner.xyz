#!/usr/bin/env sh
USER=root
CHOWN_USER=www-data
HOST=dogboner.xyz
DIR=/var/www/dogboner/ # the directory where your web site files should go

hugo && rsync --chown=${CHOWN_USER}:${CHOWN_USER} -avz --delete public/ ${USER}@${HOST}:${DIR} # delete everything on the server that's not in the local public folder

exit 0
