### install go
https://golang.org/

### install dependencies
```
go get github.com/davecgh/go-spew/spew

go get github.com/gorilla/mux

go get github.com/joho/godotenv
```

### run blockchain 
```
go run main.go
```

Make post request to 8080, example
```
// from terminal
curl -H "Content-Type: application/json" -X POST -d '{"BPM": 81}' http://localhost:8080

// reponse
 (main.Block) {
  Index: (int) 2,
  Timestamp: (string) (len=55) "2018-04-17 09:41:11.714677683 +0700 +07 m=+12.431242133",
  BPM: (int) 81,
  Hash: (string) (len=64) "27bcb46a2e975c05ff945cea2c824d26bbe81fa7c16a2aad971bafbd7662a415",
  PrevHash: (string) (len=64) "913dd3095a8298235013f5519d3d5a815d3a6e3f9fc0f3150e1ebca5519feaf4"
 }
```