# Golang RabbitMQ Reddit rss producer with Mongodb

Reddit xml rss consumer 🚀

## Installation

### Make sure you have Go installed on your system.
### Clone this repository
```git clone https://github.com/Alisalmasi/RabbitMQ-Producer.git```
### Navigate to the project directory `RabbitMQ-Producer`
### Run the project
```
 go run main.go
```

## Features

### When you make a POST request to the  endpoint ```localhost:5000/parse``` a message is send to rabbitMQ  broker and the response will be sent to consumer.
### Consumer Repo
```https://github.com/Alisalmasi/RabbitMQ-Consumer.git```

## Usage

1. Run the project.
2. Send a post request with application/json eg
```{ "url":"https://www.reddit.com/r/recipes/.rss" }```
the response of the rss will be sent to rabbitMQ and the consumer will save the response in to mongodb

## Environment Variables

- `RABBITMQ_URI`
- `RABBITMQ_QUEUE`
  
## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
