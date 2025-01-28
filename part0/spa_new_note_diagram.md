sequenceDiagram
  participant browser
  participant server

  browser->>server: Post https://studies.cs.helsinki.fi/exampleapp/new_note_spa
  activate server
  server-->>browser: 201 created
  
  note right of browser: the server sends status code 201 which means it created the message
