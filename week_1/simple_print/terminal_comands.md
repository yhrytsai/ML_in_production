1. Create python file (Check correctness in terminal)
2. Create Dockerfile
3. Create python image
    Run in terminal in Folder
    Once your code is ready and the Dockerfile is written, all you have to do is create your image to contain your application.

    """
    docker build -t simple_print .

    """
    The ’-t’ option allows you to define the name of your image. In our case we have chosen ’python-test’ but you can put what you want.
4. Run python image

    """
    docker run -it --rm simple_print
    ""