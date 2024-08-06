```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server

    User->>Browser: Enter text into the note input field
    User->>Browser: Click "Save" button
    Browser->>Server: Send POST request with new note data
    Server-->>Browser: Response with newly created note or confirmation
    Browser->>Browser: Update SPA to include new note
    Browser->>User: Display updated list of notes with new note
```