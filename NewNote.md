```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server

    User->>Browser: Enter text into the text field
    User->>Browser: Click "Save" button
    Browser->>Server: Send POST request with note data
    Server-->>Browser: Response with confirmation or updated notes
    Browser->>User: Display updated list of notes
```