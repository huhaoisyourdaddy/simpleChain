# simpleChain
A naive and simple implementation of blockchains.

### Build And Run

> run main.go


### HTTP API

- query blocks

  ```
  curl http://localhost:3001/blocks

  ```

- mine block

  ```
  curl -H "Content-type:application/json" --data '{"data" : "User post some data to block"}' http://localhost:3001/mine_block

  ```

- add peer

  ```
  curl -H "Content-type:application/json" --data '{"peer" : "ws://localhost:6001"}' http://localhost:3001/add_peer

  ```

- query peers

  ```
  curl http://localhost:3001/peers
  ```