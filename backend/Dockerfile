FROM python
WORKDIR /usr/src/app
COPY ./docker_homework/lib_catalog .
RUN pip3 install -r requirements.txt
RUN python manage.py migrate
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

