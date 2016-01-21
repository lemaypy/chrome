# chrome
Chrome Browser with Google Talk

Usage:

docker run -it \
	--net host \ # may as well YOLO
	--cpuset-cpus 0 \ # control the cpu
	--memory 512mb \ # max memory it can use
	-v /tmp/.X11-unix:/tmp/.X11-unix \ # mount the X11 socket
	-e DISPLAY=unix$DISPLAY \
	-v $HOME/Downloads:/root/Downloads \
	-v $HOME/.config/google-chrome/:/data \ # if you want to save state
	--device /dev/snd \ # so we have sound
	-v /dev/shm:/dev/shm \
	--name chrome \
	lemaypy/chrome

