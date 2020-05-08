# デプロイ方法

```sh
mvn compile exec:java \
 -Dexec.mainClass=com.google.cloud.teleport.templates.DatastoreToText \
 -Dexec.args="--runner=DataflowRunner \
              --project=dizm-beacon-receiver-v1 \
              --stagingLocation=gs://dizm-beacon-receiver-v1/staging \
              --templateLocation=gs://dizm-beacon-receiver-v1/templates/DatastoreToJSON" 
```
