FROM python
RUN mkdir /pyusbtest && \
	apt update && \
	apt -y upgrade && \
	apt -y install libusb-dev && \
	pip3 install pyusb
COPY test-pyusb.py /pyusbtest
CMD [ "python3", "/pyusbtest/test-pyusb.py" ]
