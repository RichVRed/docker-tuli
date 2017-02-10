## Tuli - A static analysis engine
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/tuli.svg)](https://hub.docker.com/r/rvannauker/tuli/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/tuli.svg)](https://hub.docker.com/r/rvannauker/tuli/) [![](https://images.microbadger.com/badges/image/rvannauker/tuli:latest.svg)](https://microbadger.com/images/rvannauker/tuli:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-tuli.svg)](https://github.com/RichVRed/docker-tuli) [![license](https://img.shields.io/github/license/RichVRed/docker-tuli.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run tuli

### Installation / Usage
1. Install the rvannauker/tuli container:
```bash
docker pull rvannauker/tuli
```
2. Run tuli through the tuli container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="tuli" "rvannauker/tuli" analyze {destination}
```

### Download the source:
To run, test and develop the TULI Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-tuli.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/tuli" --file tuli.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/tuli --help
```