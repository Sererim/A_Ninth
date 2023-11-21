```json

Server {
    id integer pk increments
    CPU integer
    RAM integer
    SSD integer
}

Customer {
    id integer pk increments
    firstname string
    givenNames string
    email string
    hashPassword string
}

Order {
    id integer pk increments
    idCustomer integer > Customer.id
    idServer integer > Server.id
    dateTimeStart datetime
    dateTimeEmd datetime
    price decimal
    RAM integer
    CPU integer
    SSD integer
    OS integer
    ipAddress string
}

```