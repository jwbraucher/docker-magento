# lamp stack built with puppet

FROM braucher/php
MAINTAINER Jeff Braucher <jeff@braucher.net>

# Install curl for downloading magento
RUN apt-get update && \
  apt-get install -y curl

# Run app
RUN mkdir -p /var/www/app
WORKDIR /var/www/app
COPY ./app* /
ENTRYPOINT ["/app"]
CMD ["start"]

