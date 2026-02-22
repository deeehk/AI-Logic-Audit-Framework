graph TD
    subgraph Input_Layer
        A[User Query / Edge Case] --> B{Contextual Tagging}
    end

    subgraph Processing_Layer_LLM
        B --> C[LLM Response Generation]
    end

    subgraph Audit_Framework_Your_System
        C --> D[Logic Deconstruction Engine]
        D --> E1[Physical Logic Check]
        D --> E2[Cultural/Historical Accuracy]
        D --> E3[Biological Constraint Audit]
        
        E1 --> F{Risk Scoring}
        E2 --> F
        E3 --> F
    end

    subgraph Output_Layer
        F --> G1[Validated Response]
        F --> G2[Hallucination Alert / Flagged]
    end

    style Audit_Framework_Your_System fill:#f9f9f9,stroke:#333,stroke-width:2px
