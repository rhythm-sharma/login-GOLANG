## Creating Simple Login API using Go and Mongodb

There are following end points :
1. /register POST ( New user registration)
2. /login POST (Existing user can login )
3. /profile GET (To get user details)


### Project setup
1. Create a new folder go-login in your $GOPATH/src directory.


2. Make your directory structure like 
    `go-login/`
    `|- controller/controller.go  - Defines handler methods of endpoints`
    `|- model/model.go       -  User and Product models`
    `|- config                  - Contains all configuration files`
    `|- db/db.go      - Contains database configuration`
    `|- main.go            - Entry point of the API`


3. install libraries for routing(mux) , database, and authentication. Run following command in terminal to install the dependencies :
`$ go get "github.com/gorilla/mux"`
`$ go get go.mongodb.org/mongo-driver/mongo`
`$ go get golang.org/x/crypto/bcrypt`