FROM nginx
RUN apt-get update
RUN apt-get install -y curl --fix-missing
RUN apt-get install -y git --fix-missing
RUN apt-get install -y nano --fix-missing
RUN apt-get install -y gnupg --fix-missing
RUN curl -sL https://deb.nodesource.com/setup_7.x | bash -
RUN apt-get install -y build-essential --fix-missing
RUN sudo apt-get update
RUN apt-get install -y nodejs --fix-missing
RUN npm install -g yarn
RUN npm install -g angular-cli
