## Diagrams

Mermaid diagram:

```mermaid
graph LR;
    A[Keep going] --> B{Failed?}
    B -- Yes --> C[Keep going!]
    B -- No --> E[Good Job!]
    C --> A
```