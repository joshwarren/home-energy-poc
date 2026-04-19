# System Architecture Overview

## High-level Component Diagram
```
+-------------------+      +-------------------------+
|    User Interface  | ---> |      Application Logic  |
+-------------------+      +-------------------------+
                                   |
                                   |
                                   v
                       +-------------------------+
                       |  Data Persistence Layer  |
                       +-------------------------+
                                   |
                                   |
                                   v
                     +--------------------------+
                     |    External API Layer     |
                     +--------------------------+
```

## Data Flow Between Components
- User inputs are processed by the User Interface, sent to Application Logic.
- Application Logic interacts with the Data Persistence Layer for storage and retrieval of data.
- Application Logic communicates with External API Layer for external data.

## Key Design Principles
- **Separation of Concerns**: Each component has a specific responsibility.
- **Scalability**: The architecture can scale as needed through modular components.

## Technology Stack Decisions
- **Frontend**: React.js
- **Backend**: Python
- **Database**: PostgreSQL

## Integration Points
- **Home Assistant**: Via REST API for device control.
- **External APIs**: REST integrations for weather data, energy pricing, etc.
