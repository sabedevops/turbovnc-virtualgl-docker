# turbovnc-virtualgl-docker

Docker container for TurboVNC and VirtualGL running NVIDIA drivers

Original Dockerfile from:
https://gitlab.com/nvidia/samples/blob/master/opengl/ubuntu16.04/turbovnc-virtualgl/Dockerfile 


1. Create the certificate self.pem

```
openssl req -new -x509 -days 365 -nodes -out self.pem -keyout self.pem
```

2. Build the image

```
docker build -t $USER/turbovnc:latest . 

```
