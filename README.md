```mermaid
graph LR
    subgraph Inputs
        A
        B
        C
    end

    subgraph Gates
        AND1([AND])
        AND2([AND])
        AND3([AND])
        OR1([OR])
    end

    subgraph Output
        F([F])
    end

    A --> AND1
    B --> AND1
    A --> AND2
    C --> AND2
    B --> AND3
    C --> AND3

    AND1 --> OR1
    AND2 --> OR1
    AND3 --> OR1
    
    OR1 --> F
