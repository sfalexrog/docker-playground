FROM sfalexrog/docker-playground:latest

# Taken from https://github.com/thewtex/docker-opengl

USER root

RUN apt-get update \
	&& DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
		git \
		libgl1-mesa-dri \
		menu \
		net-tools \
		openbox \
		ca-certificates \
		sudo \
		supervisor \
		tint2 \
		x11-xserver-utils \
		x11vnc \
		xinit \
		xserver-xorg-video-dummy \
		xserver-xorg-input-void \
		websockify \
		python \
		python3 \
		wget \
	&& wget https://bootstrap.pypa.io/get-pip.py \
	&& python get-pip.py \
	&& python3 get-pip.py \
	&& pip install supervisor-stdout \
	&& apt-get -y clean

	
USER user

