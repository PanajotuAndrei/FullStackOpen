```mermaid
flowchart
    A[HTML file] 
    B[JS file]
    C[css file]
    D[json file]
    F[loaded page]
    A-->F
    B-- Executes on the browser-->F
    C-->F
    D-->F
    