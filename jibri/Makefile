JAR = build/rootfs/opt/jitsi/jibri/jibri.jar

build: $(JAR)
	docker build $(BUILD_ARGS) -t $(JITSI_REPO)/jibri .


jar: $(JAR)

$(JAR):
	docker run -v $(shell pwd)/build-scripts:/build-scripts:ro -v $(shell pwd)/build:/build:rw -v $(shell pwd)/jibri:/src/jibri:rw jitsi/jarbuild /build-scripts/build

.PHONY: build jar
