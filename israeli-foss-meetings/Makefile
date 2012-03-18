all: israeli-2012-perl-workshop-report.xhtml

israeli-2012-perl-workshop-report.xhtml: israeli-2012-perl-workshop-report.pod
	pod2xhtml --infile "$<" --outfile "$@"

upload: all
	rsync -a -v --progress --rsh=ssh *.xhtml \
	    "$${__HOMEPAGE_REMOTE_PATH}"/telaviv.pm-meetings/
