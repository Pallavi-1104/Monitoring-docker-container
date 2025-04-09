# Monitoring-docker-container

step 1 : create docker-compose file to create container of prometheus, grafana and cadvisior
            -cadvisior is a monitoring tool used to monitor docker container resource usage 
            -prometheus scrape the metrics of cadvisior every few seconds
            -grafana visualize metrics in dashboard
         also create docker-monitoring.yml file for dashboard , prometheus.yml for datasource and prometheus.yml file for prometheus.

step 2 : Launch one ubuntu instance and connect this instance

step 3 : After that install docker on terminal and then clone the github repo

step 4 : And use the Command -- docker-compose up then it creates the containers 

step 5 : Open your browser and go to: http://localhostIP:3000 - (default login is admin / admin) to access grafana and to acess 
         prometheus use : http://localhostIP:9090

step 6 : Grafana Dashboard for Docker (cAdvisor)
        In the left sidebar where you're at, go to:
            ⚙️ Settings → Connections → Data sources
            (It's right below "Connections" — just scroll down a tiny bit and you'll see it.)
            Click "Data sources".
            Then click “Add data source”, choose Prometheus.
            In the URL field, enter:
            http://prometheus:9090
            Click “Save & Test”.

step 7 :  Import Docker Dashboard
            In the left sidebar, click on "Dashboards" → "Browse".
            Then click the “+ Import” button (top-right).
            In the Import via Grafana.com section, paste this dashboard ID:
            893
            Click Load.
            Under “Prometheus” dropdown, select the Prometheus data source you added earlier.
            Click Import.




         
