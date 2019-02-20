FROM logstash:latest

# switch to privledged user to make directory.
USER root

# Download GeoIP Data - note source may change in January 2019 see website for details.
RUN mkdir -p /usr/share/GeoIP/ && \
   curl "http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz" >> /usr/share/GeoIP/GeoLiteCity.dat.gz && \
   gunzip /usr/share/GeoIP/GeoLiteCity.dat.gz
