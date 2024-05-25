
# WhatsAPI

A simple and efficient REST API for programmatically sending WhatsApp messages using Node.js.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoint](#api-endpoint)
- [Contributing](#contributing)
- [License](#license)

## Introduction

WhatsAPI is a simple and efficient REST API for sending WhatsApp messages programmatically. It leverages Node.js and the `@builderbot/bot` and `@builderbot/provider-baileys` packages to provide a straightforward interface for WhatsApp messaging.

## Prerequisites

Make sure you have the following installed on your machine:

- Node.js (version 14 or higher)
- npm (Node package manager)

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/barrerot/WhatsAPI.git
    ```

2. Change to the cloned directory:

    ```sh
    cd WhatsAPI
    ```

3. Install the necessary dependencies:

    ```sh
    npm install
    ```

## Usage

1. Start the server:

    ```sh
    npm start
    ```

2. Follow the instructions to link the WhatsApp account you want to use with the generated QR code.

## API Endpoint

### Send WhatsApp Message

- **URL:** `/v1/messages`
- **Method:** `POST`
- **Content-Type:** `application/json`
- **Description:** Send a WhatsApp message to a specified number.

#### Request Body

| Parameter | Type   | Description                  |
|-----------|--------|------------------------------|
| number    | String | The recipient's phone number |
| message   | String | The message to send          |

#### Example Request

```sh
curl --location 'http://localhost:3001/v1/messages' --header 'Content-Type: application/json' --data '{
    "number": "34699876543",
    "message": "mensaje de prueba"
}'
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or additions.

## License

This project is licensed under the MIT License. See the [LICENSE](https://opensource.org/licenses/MIT) file for details.
