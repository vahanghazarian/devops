# localtime

# Create your Dockerfile for building your image by copying the contents below into the editor.

Copy to EditorFROM nginx:alpine
COPY . /usr/share/nginx/html

# Build our static HTML image using the build command below.

docker build -t localtime:v1 .

# Docker Run the container
docker run -d -p 800:800 localtime:v1

