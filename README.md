# processor-webapp-helm-chart
Processor Web App Helm Chart GitHub Repository Setup

Install the helm:
```bash
helm install --set DBHostName=endpoint \
             --set DBUserName=usrname \
             --set DBPassword=pwd \
             --set DBSchema=stories \
             --set KafkaServer=kafka \
             --set ESAddr=hostname:port \
             {{ .Release.Name }} ./{{ .Chart.Name }}
```

Uninstall the helm:
`helm uninstall {{ .Release.Name }}`

Check NOTES.txt for more details.

