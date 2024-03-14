sequenceDiagram
    
    Note over User,Browser: User navigates to spa
    User->>Browser: Enter https://studies.cs.helsinki.fi/exampleapp/spa
    Browser->>Server: GET spa
    Server-->>Browser: spa Files (HTML, CSS, JS)
    Note over Browser: spa initializes
    Browser->>Server: GET Notes Data
    Server-->>Browser: JSON Notes Data
    Note over Browser: Display Notes



   