参考文章：https://dev.to/koddr/build-a-restful-api-on-go-fiber-postgresql-jwt-and-swagger-docs-in-isolated-docker-containers-475j#toc


生成迁移文件
` migrate create -ext sql -dir migrations init`
生成到数据库
`migrate -verbose -path="./platform/migrations" -database "postgres://postgres:password@localhost/postgres?sslmode=disable" up`
