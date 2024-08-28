main.go: The entry point initializes the database connection and sets up the router with all the necessary routes.
config/config.go: Handles the MongoDB connection and provides the database instance.
models/pocModel.go: Defines the data structure of the poc-go items.
repositories/pocRepository.go: Contains the database queries, abstracting them away from the controller.
services/pocService.go: Implements business logic and acts as an intermediary between the controller and repository.
controllers/pocController.go: Handles HTTP requests, processes input, and returns responses.
routes/pocRoutes.go: Defines the application's endpoints and maps them to the appropriate controller functions.
tests/pocController_test.go: Contains unit tests to verify that the controller functions as expected.

poc-go/
├── backend/
│   ├── config/
│   │   └── config.go
│   ├── controllers/
│   │   └── pocController.go
│   ├── models/
│   │   └── pocModel.go
│   ├── repositories/
│   │   └── pocRepository.go
│   ├── services/
│   │   └── pocService.go
│   ├── routes/
│   │   └── pocRoutes.go
│   ├── tests/
│   │   └── pocController_test.go
│   └── main.go
└── go.mod
