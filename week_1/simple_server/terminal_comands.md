1. Create Dockerfile
2. Create python image

    """
   docker build --tag simple_server:latest .

    """
    The ’-t’ option allows you to define the name of your image. In our case we have chosen ’python-test’ but you can put what you want.
3. Run python image
    Container construction. Docker run - run a command in a new container:
    docker run [OPTIONS] IMAGE[:TAG] [COMMAND]

    - flag it - combination of -i (--interactive) + -t (--tty)
        In order to be able to interact with the container through the terminal, you need to use the -i and -t flags together.
    - The --rm flag automatically removes the container after it has finished running.
    - --name asign name to contaiter 

    """
    docker run -it --rm -p 8080:8080 --name simple_server simple_server:latest 
    ""