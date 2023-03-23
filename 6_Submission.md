```mermaid
sequenceDiagram
browser->server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
activate server
Note right of server: new note data sent as Content-type: application/json. Javascript code pushes new note to server/database
server-->>browser: Status 201 - Updated list returned
Note right of browser: Note list is re-rendered with new note via Javascript code
deactivate server
```
