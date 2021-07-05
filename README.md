# helloworld-rust-project

## Task description.

You are going to write a less-constraint blockchain simulation. In the simulation there will be n nodes (n=5 in the demo) talking to each others using [libp2p](https://github.com/libp2p/rust-libp2p) and all nodes will be started with the same code you are going to write. In addition, each node will store pairs of (pokemon_name, pokemon) where pokemon_name is a string and pokemon is an object describing the features of the pokemons. An object can be expressed, for example, as following json object:

```
{
  "color": "blue",
  "eye_num": 5,
  "nose_num": 3,
  "mouth_num": 3,
}
```

For simplicity, the node can store those objects in memory.

For the node, you will be also implementing a service to receive a transaction (POST/GET) from end user where POST transaction is to create a new pokemen or update an existing one, and GET transaction with the given `name` is to return the json object of that pokemon `name`. You can use[ json_rpc](https://github.com/paritytech/jsonrpc) for this service.

For your productivity, you can try to use handy-library to derive Serialize/Deserialize the json object.

## Delivery

1. Github repo
2. Instruction to run the demo will be written in the README.md file.
