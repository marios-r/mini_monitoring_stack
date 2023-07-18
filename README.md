# Mini Monitoring Stack

Basic setup of Prometheus, AlertManager and Grafana with docker-compose configured to send an email when your application is offline as well as to show a dashboard with the uptime.
All you need to do is edit the variables in email_configs on file alertmanager/alertmanager.yml as well as the targets in scrape_configs on file prometheus/prometheus.yml appropriately.

Note that if you use Gmails SMTP to try it out as I did, you will have to create and use an app password on your Gmail as nowadays two step verification won't allow you to use your normal password.

Run:
```
docker compose up
```