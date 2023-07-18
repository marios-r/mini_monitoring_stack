# Mini Monitoring Stack

Basic setup of Prometheus, AlertManager and Grafana with docker-compose configured to send an email when your application is offline as well as to show a dashboard with the uptime.
<img width="919" alt="Screenshot 2023-07-18 at 3 33 11 PM" src="https://github.com/marios-r/mini_monitoring_stack/assets/18104126/deddee73-f54b-496d-99a0-fd3e5ab3487e">

All you need to do is edit the variables in email_configs on file alertmanager/alertmanager.yml as well as the targets in scrape_configs on file prometheus/prometheus.yml appropriately.

Note that if you use Gmails SMTP to try it out as I did, you will have to create and use an app password on your Gmail as nowadays two step verification won't allow you to use your normal password.

**Run:**
```
docker compose up
```
