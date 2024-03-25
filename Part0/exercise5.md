```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: GET Request
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET Request
    activate server
    server-->>browser: css file
    deactivate server

    browser->>server: GET Request
    activate server
    server-->>browser: the JavaScript file
    deactivate server

    Note right of browser: The browser executes javascript file locally and takes 

    browser->>server: GET request
    activate server
    server-->>browser: [updated json file with new data ]
    deactivate server

    Note right of browser: JS fetches the notes from the server as JSON data and adds HTML elements for displaying the notes
    