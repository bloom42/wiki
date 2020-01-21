# Go

**Why go is not optimal:**

* Pointers
* Lack of immutability
* No algebraic data types
* Imperative paradigm

## Commands

See https://news.ycombinator.com/item?id=20869324
```sh
$ go env -w GOFLAGS=-mod=vendor
$ go env -w GOPROXY="direct"
$ go env -w GOSUMDB="off"
```


## Guides

### How to access a SQL Database

comment acceder a la db

pq orm: https://github.com/go-pg/pg
postgres driver: https://github.com/go-pg/pg
sqlx: https://github.com/jmoiron/sqlx (pas mis a jour)
gorm: https://github.com/jinzhu/gorm



ce qui semble se dessiner:
sqlx, avec repository pattern, comme ca on peut switcher / alterner

pattern

domain
- mode
- command (ou use cases?)
- query (repositories?)
handler

et les repositories ?


on met la logique ‘gloable’ dans les handler, et ceux ci ne font que appeler des groupement de commandes




he file service.go represents the Use Case layer, as defined by Uncle Bob. In the file we have the interface Service and his implementation. The Service interface is:

———————

les handler sont nos controller

dans le domaine on retrouve les commandes, les notifs et les modeles




## Resources

### Crypto

* https://www.alexedwards.net/blog/how-to-hash-and-verify-passwords-with-argon2-in-go

### Modules

* https://vyskocil.org/blog/go-111-modules-monorepo-and-shared-code/
* https://www.reddit.com/r/golang/comments/9viv50/how_i_solved_go_111_modules_private_monorepo_and/
* https://github.com/go-modules-by-example/index/blob/master/009_submodules/README.md
* https://github.com/sotah-inc/server/tree/master/app
* https://blog.digitalocean.com/cthulhu-organizing-go-code-in-a-scalable-repo/
* https://arslan.io/2019/08/02/why-you-should-use-a-go-module-proxy/

### Database

* https://jmoiron.github.io/sqlx/
* https://www.alexedwards.net/blog/organising-database-access
* https://github.com/golang-migrate/migrate#use-in-your-go-project
* https://www.w3resource.com/sqlite/sqlite-data-types.php
* https://github.com/whiteheadrj/goDataStoreExamples/blob/master/example4/store.go
* https://husio.github.io/blog/accessing-data-in-go/
* https://medium.com/avitotech/how-to-work-with-postgres-in-go-bad2dabd13e4
* https://astaxie.gitbooks.io/build-web-application-with-golang/en/05.4.html
* https://blog.digitalocean.com/create-a-simple-contacts-list-with-go/
* https://jbrandhorst.com/post/postgres/
* https://www.calhoun.io/using-postgresql-with-go/
* https://www.compose.com/articles/accessing-relational-databases-using-go/
* https://medium.com/@ChadITNP/golang-database-access-d603ceeb266f
* https://hackernoon.com/how-to-work-with-databases-in-golang-33b002aa8c47
* http://go-database-sql.org/
* https://docs.microsoft.com/fr-fr/azure/postgresql/connect-go
* https://www.alexedwards.net/blog/using-postgresql-jsonb
* https://kb.objectrocket.com/postgresql/web-app-with-go-and-postgresql-update-record-in-postgresql-using-golang-733

### Code organization

* * https://rakyll.org/style-packages/
* https://medium.com/manato/clean-architecture-with-go-bce409427d31
* https://medium.com/@eminetto/clean-architecture-using-golang-b63587aa5e3f
* https://medium.com/manato/clean-architecture-with-go-bce409427d31
* https://hackernoon.com/trying-clean-architecture-on-golang-2-44d615bf8fdf
* https://medium.com/@hatajoe/clean-architecture-in-go-4030f11ec1b1

### Mobile

* https://medium.com/@AndroidAdvance/running-go-from-android-ios-tutorial-7f1d456c5b0f
* https://sites.google.com/a/athaydes.com/renato-athaydes/posts/buildingamobilefrontendforagoapplicationusingflutter

### CGO

* https://gist.github.com/helinwang/2c7bd2867ea5110f70e6431a7c80cd9b
* https://golang.org/cmd/cgo/
* https://blog.golang.org/c-go-cgo
* https://stackoverflow.com/questions/35507467/cgo-how-to-free-memory-allocated-in-c-using-malloc-from-go-to-avoid-memory-leak
* https://karthikkaranth.me/blog/calling-c-code-from-go/
* https://dave.cheney.net/tag/cgo
* http://akrennmair.github.io/golang-cgo-slides/#1

### Other


* https://github.com/asaskevich/govalidator
* https://www.digitalocean.com/community/tutorials/how-to-format-strings-in-go
* https://medium.com/@benbjohnson/structuring-applications-in-go-3b04be4ff091#9e7e
* https://yourbasic.org/golang/switch-statement/
* https://www.yellowduck.be/posts/injecting-build-time-variables/
* https://medium.com/statuscode/how-i-write-go-http-services-after-seven-years-37c208122831
* https://code.tutsplus.com/tutorials/json-serialization-with-golang--cms-30209
* https://eagain.net/articles/go-dynamic-json/
* https://eagain.net/articles/go-json-kind/
* https://arslan.io/2017/09/14/the-ultimate-guide-to-writing-a-go-tool/
* https://tech.labs.oliverwyman.com/blog/2011/04/30/using-the-syntax-tree-in-go/
* https://medium.com/@chemidy/create-the-smallest-and-secured-golang-docker-image-based-on-scratch-4752223b7324
* https://medium.com/@shijuvar/building-microservices-with-event-sourcing-cqrs-in-go-using-grpc-nats-streaming-and-cockroachdb-983f650452aa
* https://ewanvalentine.io/microservices-in-golang-part-10/
* https://blog.golang.org/pipelines
* https://www.gmarik.info/blog/2016/experimenting-with-golang-pipelines/
* https://github.com/trustmaster/goflow
* https://appliedgo.net/flow/
* https://github.com/chrislusf/gleam
* https://fr.slideshare.net/AntonStepanenko/flow-based-programming-in-golang
* https://aws.amazon.com/fr/step-functions/
* https://github.com/Pungyeon/clean-go-article#Introduction-to-Clean-Code
