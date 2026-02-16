# Monolithic Architecture Example

This example demonstrates an exhaustive 10-aspect visualization of a typical monolithic web application.

## Architecture Pattern Detected

**Pattern:** Layered Monolith with MVC
**Framework:** Web framework (HTTP handling, routing)
**Database:** Relational (PostgreSQL)
**Key Characteristics:**
- Single deployable unit
- Layered architecture (Controller → Service → Repository)
- Session-based authentication
- Synchronous request/response

## Aspects Generated

| Aspect | File | Description |
|--------|------|-------------|
| Context | `monolith_context.dot` | External users, system boundaries |
| Components | `monolith_components.dot` | Module layers |
| Types | `monolith_types.dot` | Core domain models |
| Flow | `monolith_flow.dot` | Request lifecycle |
| Concurrency | `monolith_concurrency.dot` | Thread pool, sync model |
| Storage | `monolith_storage.dot` | DB schema, cache |
| Security | `monolith_security.dot` | Auth flow, trust zones |
| Deployment | `monolith_deployment.dot` | Single server deployment |
| Memory | `monolith_memory.dot` | Heap, stack, GC regions |
| State | `monolith_state.dot` | Lifecycle, transitions |

## Key Design Decisions

1. **Layered Architecture**: Clear separation between HTTP handling and business logic
2. **Synchronous Processing**: Single-threaded request handling with connection pooling
3. **Relational Database**: ACID transactions for data integrity
4. **Session-Based Auth**: Server-side session storage

## Visualization Notes

- External boundary shown in red
- Application services in blue
- Domain layer in green (core business logic)
- Data layer in orange
- All edges use orthogonal lines (right angles)
- Edge labels use `xlabel`, not `label`
