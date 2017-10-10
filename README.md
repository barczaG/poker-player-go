poker-player-go
===============

Go client skeleton for Lean Poker. For more information visit: http://leanpoker.org 

## Usage instructions

### Ingredients

See [Deploying Go Apps on Heroku](https://devcenter.heroku.com/articles/deploying-go#prerequisites)

### Workflow

0. Make sure you have $GOPATH correctly: https://golang.org/doc/code.html
1. Fork this repo (Leanpoker platform will do this for you) eg: https://github.com/Hunrik/poker-player-goglig
2. `go get YOUR_FORK` eg: `go get github.com/Hunrik/poker-player-goglig`
3. `cd $GOPATH/src/YOUR_FORK` eg: `cd $GOPATH/src/github.com/Hunrik/poker-player-goglig`
3. Fix import path in your fork 
eg replace all occurence of `github.com/lean-poker/poker-player-go` to `github.com/Hunrik/poker-player-goglig`
at:
https://github.com/barczaG/poker-player-go/blob/master/player-service.go#L11
https://github.com/barczaG/poker-player-go/blob/master/player-service.go#L12
https://github.com/barczaG/poker-player-go/blob/master/Godeps/Godeps.json#L2
https://github.com/barczaG/poker-player-go/blob/master/player/player.go#L3
4. Update dependencies with `godep save ./...`
5. Inspect and commit changes
6. Push
7. Enjoy
