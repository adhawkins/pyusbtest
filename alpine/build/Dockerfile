FROM python:alpine
RUN mkdir /pyusbtest && \
	apk update && \
	apk upgrade && \
	apk add libusb-dev libusb-compat-dev && \
	pip3 install pyusb
COPY test-pyusb.py /pyusbtest
CMD [ "python3", "/pyusbtest/test-pyusb.py" ]
