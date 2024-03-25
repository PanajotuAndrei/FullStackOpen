```mermaid
flowchart
    O[HTML]-->
    A[Form Submit] 
    B[Server JS]
    A-->POST{POST}-->B-- CODE 201-->A
    B--updates notes through the command notes.push(note)--> notes-->server--rerender-->O
    