# Local Run
~~~~
docker build -t beautiful-jekyll CenikLab.github.io

docker run -d -p 4000:4000 --name beautiful-jekyll -v CenikLab.github.io:/srv/jekyll beautiful-jekyll
~~~~
