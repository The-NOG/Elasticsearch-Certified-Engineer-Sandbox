# Elasticsearch Certified Engineer Sandbox
 Elasticsearch sandbox for studying for the Elasticsearch Certified Engineer Exam. All in one inside docker!

## What is this?
 This is a docker compose used to setup an environment that is perfect for studying for the Elasticsearch Certified Engineer exam. It has two clusters, main and remote. The main cluster has 3 ES nodes and one Kibana node. This cluster will use the typical Elasticsearch and Kibana ports (9200/5601). The remote cluster is a simple one node Elasticsearch and Kibana. This cluster has ports exposed to the host that are +1, so 9201 and 5602

 ## Why did you...
- **Set the version to 8.1.3?** The current exam is still on elasticsearch 8.1
- **Set the elastic passwords to *elastic*?** It's a simple environment for studying, don't use for anything you care about or overthink it.
- **Activate the trial?** The trial is required for cross cluster replication which is an exam topic.

## Other resources
- Highly recommend the [repo by mr1716](https://github.com/mr1716/Elastic-Certified-Engineer-Exam-8.1).
- The course on A cloud Guru/plural sight is pretty good. It was made for 7.13, but should be *mostly* relevant
- The training from Elasticsearch is excellent. If you can swing it or make your company pay for it go for it.

## Credit
Credit where credit is due, the base of this is from [Elasticsearch themselves](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html#docker-compose-file). I just modified it to have the extra small cluster for learning the cross cluster requirements.