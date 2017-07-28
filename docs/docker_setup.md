## Setup Docker on Ubuntu

https://www.howtoforge.com/tutorial/how-to-install-jenkins-with-apache-on-ubuntu-16-04/

## Steps to run Docker
1. From Ubuntu, create folder: /home/hiep/my_dockers
2. Create docker file: "selen_docker_file1" under /home/hiep/my_dockers (see attached selen_docker_file1)
3. Copy file "xvfb.init" to /home/hiep/my_dockers
4. Copy file "selen_test.py" to /home/hiep/my_dockers
5. Make sure "chromedriver" download and put under /home/hiep/my_dockers
6. Build docker image command: docker build -f "selen_docker_file1"
7. To test docker image build: docker run -t -i --rm selen_docker_file1 ls
8. To run example selenium test case inside docker image and mount selen_test.py:
   * docker run -rm -v /home/hiep/my_dockers:/home/hiep/my_dockers -it selen_image /bin/bash -c “python /home/hiep/my_dockers/selen_test.py”
9.  To run selenium test with robot framework:
will be continued

