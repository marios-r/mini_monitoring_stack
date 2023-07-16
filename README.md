# Mini Monitoring Stack

Basic setup of Prometheus and AlertManager with docker-compose configured to send an email when your application is offline.
All you need to do is edit the variables in email_configs on file alertmanager/alertmanager.yml as well as the targets in scrape_configs on file prometheus/prometheus.yml appropriately.

Optionally, you may also want to change the job name on prometheus/prometheus.yml and prometheus/alert.yml

Note that if you use Gmails SMTP to try it out as I did, you will have to create and use an app password on your Gmail as nowadays two step verification won't allow you to use your normal password.