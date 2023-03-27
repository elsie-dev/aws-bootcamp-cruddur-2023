 FROM python:3.10-slim-buster
 ENV PORT=4567
 WORKDIR /backend-flask

 COPY requirements.txt requirements.txt

 COPY envoy.yaml /etc/envoy/envoy.yaml
 RUN pip3 install -r requirements.txt
 RUN chmod go+r /etc/envoy/envoy.yaml

 COPY . .

 ENV FLASK_ENV=development

 EXPOSE ${PORT}
 CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]

#  CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567", "envoy.yaml"]

# FROM envoyproxy/envoy:dev-345752d60cda2f2c1c47e36cdd30752b3f9d6880
# COPY envoy.yaml /etc/envoy/envoy.yaml
# RUN chmod go+r /etc/envoy/envoy.yaml