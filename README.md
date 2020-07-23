# localtime

# Create your Dockerfile for building your image by copying the contents below into the editor.

Copy to EditorFROM nginx:alpine
COPY . /usr/share/nginx/html

# Build our static HTML image using the build command below.

docker build -t localtime:v1 .

# Docker Run the container
docker run -d -p 5000:80 localtime:v1

# Open index.html
http://95.216.217.20:5000/index.html

# Open monitoring.html
http://95.216.217.20:5000/monitoring.html

