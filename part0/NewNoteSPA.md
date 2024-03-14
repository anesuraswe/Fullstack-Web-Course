sequenceDiagram
    Note over User,Browser: User adds new note
    User->>Browser: Submit new note
    Browser->>Server: POST new note content
    Server-->>Browser: JSON Updated Notes Data
    Note over Browser: Update and Display Notes
    Browser->>Server: GET spa
    Server-->>Browser: spa Files (HTML, CSS, JS)
    Note over Browser: spa initializes
    Browser->>Server: GET Notes Data
    Server-->>Browser: JSON Notes Data
    Note over Browser: Display Notes