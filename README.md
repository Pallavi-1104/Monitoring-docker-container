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
<img width="945" alt="{2024516E-DDD6-4DD5-9DA2-D2720243D36C}" src="https://github.com/user-attachments/assets/e8dc6c6b-3931-4d2c-88f2-88e71b2db874" />
<img width="960" alt="{BDDD8EB5-01FF-4F41-8A0D-EF65536E467C}" src="https://github.com/user-attachments/assets/41c63151-8d78-4e3a-a227-9a25f69892cd" />
<img width="956" alt="{0E2DFA87-BECE-41EC-B88B-DF06D3DA52E4}" src="https://github.com/user-attachments/assets/8db7cfbf-9ddd-46a4-b089-196fb5e877b0" />
<img width="959" alt="{5A33C695-AF69-4539-8D3D-AC2A3CBED133}" src="https://github.com/user-attachments/assets/4f1978df-85de-4037-a085-49121e73b8de" />






         
