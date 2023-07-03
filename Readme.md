# Warehouse Picking Routes Sort BE

Node.js and Express application written in TypeScript that provides a simple HTTP server with only one endpoint for managing warehouse picking routes. Run on external API but now will need own DB (not yet done)

## Features

- Fetches warehouse data from an external API
- Provides an endpoint for order picking based on lowest product quantity position and efficient labor usage
- Calculates shortest path using Euclidean distance
- Error handling
- Tests with Jest

## Prerequisites

- Node.js
- NPM

## Installation

1. Clone the repository:

```sh
git clone https://github.com/Vitto44/warehouse_NodeJS_BE.git
```

2. Change to the project directory:

```sh
cd warehouse_NodeJS_BE
```

3. Install the required dependencies:

```sh
npm install
```

4. Create a .env file in the project root directory and add the required environment variables:
   (was designed to run on external API, the API is now down, so database will need to be added. Currently isn't)

```sh
API_KEY=API_key
PORT=3000
```

Replace API_key with the actual API key.

### Running the application in development mode

To start the application in development mode, run:

```sh
npm run dev
```

The server will start on the specified port (default is 3000).

### Building and running the application for production

1. Build the application:

```sh
npm run build
```

This command will generate the transpiled JavaScript code into the dist folder.

2. Start the production server:

```sh
npm run prod
```

The server will start on the specified port (default is 3000).

### Running tests

To run the unit tests, execute:

```sh
npm test
```

This will run the test suite using Jest and output the results.
