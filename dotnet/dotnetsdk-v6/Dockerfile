FROM ubuntu:latest
RUN apt-get update -y 
RUN apt-get upgrade -y
RUN apt-get -y install curl
RUN curl https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb
#RUN curl https://packages.microsoft.com/config/ubuntu/20.04/prod.list
#RUN apt-get update -y 
##RUN apt-cache dump | grep dotnet-sdk-5.0
RUN apt install dotnet-sdk-6.0 -y
#RUN dotnet --list-sdks
CMD ["dotnet", "--list-sdks"]