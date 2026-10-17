# ParkPulse — Process Diagrams

## Payment and rewards

```mermaid
flowchart TD
    A["End parking session"] --> B["Calculate parking and charging costs"]
    B --> C{"Use a benefit?"}

    C -->|No| F["Display final amount"]
    C -->|Yes| D["Select one discount or voucher"]
    D --> E{"Benefit valid?"}

    E -->|No| X["Show error and allow another choice"]
    X --> C
    E -->|Yes| F

    F --> G["Simulate payment"]
    G --> H{"Payment successful?"}

    H -->|No| I["Preserve voucher and allow retry"]
    I --> F

    H -->|Yes| J["Record completion exactly once"]
    J --> K{"Eligible paid session?"}

    K -->|No| N["Show receipt and rewards"]
    K -->|Yes| L["Credit one stamp exactly once"]
    L --> M{"Six stamps reached?"}

    M -->|No| N
    M -->|Yes| O["Issue one voucher and reset stamp counter"]
    O --> N
```

## Notes
- Availability and payments are simulated.
- A free-parking reward session does not earn another stamp.
- Repeated confirmation must not duplicate rewards.
