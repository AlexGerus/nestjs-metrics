Do without scaledobject file and then apply it after installation
<b>helm install nestjs-metrics .</b>
<b>kubectl apply -f templates/scaledobject.yaml </b>

To get password for grafana:
<b>kubectl get secret nestjs-metrics-grafana -o jsonpath="{.data.admin-password}" | base64 --decode; echo</b>
