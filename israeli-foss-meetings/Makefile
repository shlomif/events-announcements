all:

upload:
	rsync -a -v --progress --rsh=ssh *.xhtml \
	    "$${__HOMEPAGE_REMOTE_PATH}"/telaviv.pm-meetings/
