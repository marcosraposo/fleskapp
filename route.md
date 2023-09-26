# Comandos

oc project flask-uat
oc create route edge flask-itg --hostname flask.itg.ocpcloud.mec.gov.br --service flask-service-uat --port 8080
oc label route flask-itg env=itg

oc project flask-uat
oc create route edge flask-pcr --hostname flask.pcr.ocpcloud.mec.gov.br --service flask-service-uat --port 8080
oc label route flask-pcr env=pcr

oc project flask-uat
oc create route edge flask-srv --hostname flask.srv.ocpcloud.mec.gov.br --service flask-service-uat --port 8080
oc label route flask-srv env=srv
