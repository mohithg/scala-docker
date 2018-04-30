# Scala

## Running docker
- Build docker as `docker build . --tag=scala`
- Run the docker as `docker run -itd scala`

- Then you can `docker container exec -it scala /bin/bash`
- You will get access to machine and start playing with sbt

## Running with local volume 
- Assuming you have cloned this directory in ~
- `docker run --name="scala" -v ~/scala/app:/app  -itd scala`

## Testing
- Once you are inside the container
- Run `scala hello.scala`
- You should see Hello World!

Now you have your volume mapped to docker container and you can exec into the
container and start running your scala programs.
You can use your preferred IDE to start putting files in app directory and it
will be reflected there in the container
