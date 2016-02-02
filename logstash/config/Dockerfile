FROM logstash:latest

# Download GeoIP Data
RUN curl "http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz" >> /config/GeoLiteCity.dat.gz && \
  gunzip /config/GeoLiteCity.dat.gz
