# Accelerator Log

## Options
```json
{
  "gitBranch" : "main",
  "gitRepo" : "https://github.com/tmm-tanzu/spring-sensors-rabbit.git",
  "projectName" : "spring-sensors-rabit",
  "publisherRepository" : "gcr.io/taaron-1/spring-sensors-publisher",
  "title" : "Tanzu Sensor Database",
  "workloadType" : "web"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [GITREPO->https://github.com/t...(truncated), main->main, WORKLOADTYPE->web]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [src/main/resources/application.yaml]
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml matched [src/main/resources/application.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [src/main/resources/application.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [Sensor Database->Tanzu Sensor Databas...(truncated)]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [demo/publisher-deployment.yaml, demo/publisher-image.yaml]
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-deployment.yaml matched [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug demo/publisher-image.yaml matched [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/cluster.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug rabbit/rbac.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorData.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorRepository.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsApplication.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsDataSink.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/org/tanzu/demo/SensorsUiController.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.yaml didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/static/tanzu.css didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/templates/index.html didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug src/test/java/org/tanzu/demo/SensorsApplicationTests.java didn't match [demo/publisher-deployment.yaml, demo/publisher-image.yaml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┗ ┗ ┗ ┗  Info Will replace [dev.local/spring-sensors-publisher->gcr.io/taaron-1/spri...(truncated)]
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
