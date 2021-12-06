FROM postgres
RUN echo "host myproject myprojectuser 0.0.0.0/0 md5" >> pg_hba.conf
ENV POSTGRES_USER=myprojectuser
ENV POSTGRES_DB=myproject
ENV POSTGRES_PASSWORD=password
CMD ["postgres"]
