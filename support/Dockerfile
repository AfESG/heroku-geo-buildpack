FROM heroku/heroku:16-build
MAINTAINER cyberdelia

RUN apt-get -q update
RUN apt install -y python-pip
RUN pip install awscli --upgrade

ADD package_gdal package_gdal
ADD package_geos package_geos
ADD package_proj package_proj
ADD geo-build geo-build

CMD ./geo-build