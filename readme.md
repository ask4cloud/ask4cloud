graph TD
    A[Environment (Branch)] --> B[System (Top-level Folder)]
    B --> C[Subsystem (Subfolder)]
    C --> D[Type (File Type/Category)]
    
    subgraph Dev [Development Branch]
        B1[App1] --> C1[Service1] --> D1[Source Code]
        B1 --> C2[Service2] --> D2[Configuration]
        B2[App2] --> C3[Service1] --> D3[Documentation]
    end

    subgraph Test [Test Branch]
        B3[App1] --> C4[Service1] --> D4[Source Code]
        B3 --> C5[Service2] --> D5[Configuration]
        B4[App2] --> C6[Service1] --> D6[Documentation]
    end

    subgraph Prod [Production Branch]
        B5[App1] --> C7[Service1] --> D7[Source Code]
        B5 --> C8[Service2] --> D8[Configuration]
        B6[App2] --> C9[Service1] --> D9[Documentation]
    end
