#Use Python Image

FROM python:3

# Install apt dependencies

RUN sudo apt update && install python3-pip
 
# Copy contents into image

COPY . . 
 
# run pip dependencies

RUN pip3 install flask && pip3 install pymysql && pip3 install flask-sqlalchemy
 
# Expose correct port

EXPOSE 5000

# Create an entrypoint

ENTRYPOINT ["python3", "app.py"]

