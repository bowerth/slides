# DECKTAPE=/home/xps13/decktape-1.0.0/

.PHONY: all
all: nsoapi-1080p.pdf # nsoapi-720p.pdf # nsoapi-1280x960.pdf nsoapi-1280x1024.pdf nsoapi-16to10.pdf 

nsoapi-1080p.pdf: ../nsoapi/index.html
	# $(DECKTAPE)/phantomjs $(DECKTAPE)/decktape.js -s 1920x1080 reveal ../nsoapi/index.html nsoapi-1080p.pdf
	docker run --rm --net=host -v `pwd`:/slides astefanutti/decktape http://localhost:8080/nsoapi/ nsoapi-1080p.pdf

# nsoapi-720p.pdf: ../nsoapi/index.html
# 	# $(DECKTAPE)/phantomjs $(DECKTAPE)/decktape.js -s 1280x720 reveal ../nsoapi/index.html nsoapi-720p.pdf
# 	$(DECKTAPE)/phantomjs $(DECKTAPE)/decktape.js -s 1280x720 remark ../nsoapi/index.html nsoapi-720p.pdf

# nsoapi-16to10.pdf: ../nsoapi/index.html
# 	$(DECKTAPE)/phantomjs $(DECKTAPE)/decktape.js -s 2560x1600 reveal ../nsoapi/index.html nsoapi-16to10.pdf

# nsoapi-4to3.pdf: ../nsoapi/index.html
# 	$(DECKTAPE)/phantomjs $(DECKTAPE)/decktape.js -s 1280x960 reveal ../nsoapi/index.html nsoapi-4to3.pdf

# nsoapi-1280x1024.pdf: ../nsoapi/index.html
# 	$(DECKTAPE)/phantomjs $(DECKTAPE)/decktape.js -s 1280x1024 reveal ../nsoapi/index.html nsoapi-1280x1024.pdf
