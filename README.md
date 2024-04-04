# Sentrify API Documentation

Welcome to the Sentrify API documentation. This guide is designed to help developers understand how to interact with the Sentrify API to leverage its capabilities.

## Base URL

The base URL for the Sentrify API is `https://api.sentrify.org/`.

## Getting Started

To use the Sentrify API, you first need an API key. To obtain an API key:

1. Join the Sentrify support Discord server at `discord.gg/sentrify`.
2. Use the `/api` command to request an API key.

## Endpoints

### `/`
- **Method**: GET
- **Description**: Returns the status of the API.

### `/api/valid`
- **Method**: GET
- **Description**: Checks if an API key is valid.
- **Parameters**:
  - `api_key`: The API key to validate.

### `/api/info`
- **Method**: GET
- **Description**: Provides information about the user associated with the given API key.
- **Parameters**:
  - `api_key`: The API key to look up.

### `/api/ai/models`
- **Method**: GET
- **Description**: Lists all AI models available in the database.
- **Parameters**:
  - `api_key`: The API key for authentication.

### `/api/ai/chat`
- **Method**: GET
- **Description**: Allows chatting with an AI model.
- **Parameters**:
  - `api_key`: The API key for authentication.
  - `prompt`: The prompt to send to the AI.

## Rate Limiting

The Sentrify API implements rate limiting to ensure fair usage. Each endpoint may have different limits. For example, the `/api/ai/chat` endpoint allows up to 100 requests per day per API key, while other endpoints may have different limits. Exceeding these limits will result in a `429 Too Many Requests` response.

For more information on specific rate limits, please refer to the endpoint documentation or contact support through the Discord server.
