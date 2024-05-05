```mermaid
    sequenceDiagram
        participant user
        participant browser
        participant server
    
        user->>browser: Clicks save
        browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
        activate server
        server-->>browser: STATUS: 201 Created
        deactivate server
        Note left of browser: Browser updates view with new note without reloading page
```
