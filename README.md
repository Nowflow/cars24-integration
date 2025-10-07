# Cars24 Integration API

This repository contains OpenAPI specifications for Cars24 integration services, providing APIs for agent management and partner hub scheduling.

## 📚 API Documentation

View the interactive API documentation with Swagger UI:

**🔗 [View Swagger Documentation](https://nowflow.github.io/cars24-integration/)**

## 📋 Available APIs

### 1. Cars24 Integration API (`cars24.yaml`)
- **Purpose**: Agent management and scrubbing services
- **Version**: 1.0.0
- **Base URL**: 
  - Production: `https://api.cars24.com/v1`
  - Staging: `https://staging-api.cars24.com/v1`

#### Key Endpoints:
- `POST /agents/scrub` - Filter agents to get online agents based on call ID, schedule ID, and metadata

### 2. Partner Hub API (`popin.yaml`)
- **Purpose**: Partner hub schedule management
- **Version**: 1.0.0
- **Base URL**: 
  - Production: `https://api.example.com`
  - Staging: `https://staging.api.example.com`

#### Key Endpoints:
- `POST /api/v1/partner-hub/schedule` - Create a new schedule
- `PUT /api/v1/partner-hub/schedule/{schedule_id}` - Reschedule an existing schedule
- `DELETE /api/v1/partner-hub/schedule/{schedule_id}` - Cancel a schedule
- `GET /api/v1/partner-hub/agents` - Get online agents for a group

## 🚀 Quick Start

1. **View Documentation**: Visit the [Swagger UI](https://nowflow.github.io/cars24-integration/) to explore the APIs interactively
2. **Local Development**: Clone this repository and open `index.html` in your browser to view the documentation locally
3. **API Testing**: Use the "Try it out" feature in Swagger UI to test endpoints directly

## 🔐 Authentication

### Cars24 Integration API
- **API Key**: `X-API-Key` header
- **Bearer Token**: JWT token in `Authorization` header

### Partner Hub API
- **Bearer Token**: JWT token in `Authorization` header

## 📁 Project Structure

```
cars24-integration/
├── README.md           # This file
├── index.html          # Swagger UI interface
├── cars24.yaml         # Cars24 Integration API specification
└── popin.yaml          # Partner Hub API specification
```

## 🛠️ Development

The project uses:
- **OpenAPI 3.0.3** for API specifications
- **Swagger UI** for interactive documentation
- **GitHub Pages** for hosting the documentation

## 📞 Support

For API support and questions:
- **Cars24 Integration API**: dev@cars24.com
- **Partner Hub API**: support@example.com

## 📄 License

This project is part of the Cars24 integration ecosystem. Please contact the development team for licensing information.
