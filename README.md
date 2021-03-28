## People distribution using FogFlow
### How to run
#### Requirements
* node
* angular
* docker
* docker-compose
* curl

If you want to modify the fog function:
* maven
* account on docker hub

#### Run
Update with your ip (if running on your machine only update the ones with *):
* main/start.sh
* main/config.json * (update with your internal ip)
* main/prometheus.yml * (update with your internal ip)
* dashboard/proxy.js * (update with your internal ip, PROVIDING_APPLICATION only)
* dashboard/src/app/app.component.ts
* dashboard/src/app/app.module.ts

Run inside main folder:
```console
./start.sh
```
You can then find FogFlow [here][1].

You can then find Grafana [here][2] (data visualization tool, username & password: admin).
How to configure:
![grafana](main/grafana.png)


Wait 15 secs.

Run inside dashboard folder:
```console
npm run start_dashboard
npm run start_server
```
You can then find the people counter dashboard [here][3].

[1]: http://localhost
[2]: http://localhost:3000
[3]: http://localhost:4200

#### Docs

Inside docs folder.
