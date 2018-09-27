3.1
Users
curl -i -XPOST -H"Content-Type: application/json" localhost:8083/registration -d'{"name": "Pete"}'
Projects
curl -i -XPOST -H"Content-Type: application/json" localhost:8083/projects -d"{\"name\": \"Basket Weaving\", \"accountId\": ${ACCOUNT_ID}}"
Allocations
curl -i -XPOST -H"Content-Type: application/json" localhost:8081/allocations -d"{\"projectId\": ${PROJECT_ID}, \"userId\": ${USER_ID}, \"firstDay\": \"2015-05-17\", \"lastDay\": \"2015-05-18\"}"
Stories
curl -i -XPOST -H"Content-Type: application/json" localhost:8082/stories -d"{\"projectId\": ${PROJECT_ID}, \"name\": \"Find some reeds\"}"
Time Entries
curl -i -XPOST -H"Content-Type: application/json" localhost:8084/time-entries/ -d"{\"projectId\": ${PROJECT_ID}, \"userId\": ${USER_ID}, \"date\": \"2015-05-17\", \"hours\": 6}"

These are rest endpoint
3.2--
https://docs.pivotal.io/spring-cloud-services/2-0/common/client-dependencies.html
curl https://spring-cloud-broker.apps.nonprod.dryice01.in.hclcnlabs.com/info -k