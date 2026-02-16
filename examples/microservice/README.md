# Microservice Architecture Example

This example demonstrates an exhaustive 8-aspect visualization of a typical microservice architecture.

## Architecture Pattern Detected

**Pattern:** Microservices with API Gateway
**Communication:** REST + gRPC + Message Queue
**Database:** Polyglot (separate DB per service)
**Key Characteristics:**
- Independent deployable services
- Service mesh / API Gateway
- Event-driven communication
- Decentralized data management

## Aspects Generated

| Aspect | File | Description |
|--------|------|-------------|
| Context | `microservice_context.dot` | External users, service boundaries |
| Components | `microservice_components.dot` | Service inventory |
| Types | `microservice_types.dot` | Service contracts, DTOs |
| Flow | `microservice_flow.dot` | Request choreography |
| Concurrency | `microservice_concurrency.dot` | Event processing |
| Storage | `microservice_storage.dot` | Polyglot persistence |
| Security | `microservice_security.dot` | Service auth, mTLS |
| Deployment | `microservice_deployment.dot` | Container orchestration |

## Key Design Decisions

1. **API Gateway Pattern**: Central entry point for all clients
2. **Database per Service**: Each service owns its data
3. **Event-Driven**: Async communication via message queue
4. **Circuit Breaker**: Resilience patterns for inter-service calls
5. **Service Discovery**: Dynamic service registration

## Visualization Notes

- Each service is a separate cluster
- API Gateway as central entry point
- Message queue for async communication
- Direct gRPC for sync calls between services
