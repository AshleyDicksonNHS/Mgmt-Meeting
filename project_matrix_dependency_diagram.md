# Payment & Pricing Team Project Matrix

The project matrix describes the lines of responsibility for each piece of work across the team. Here, I attempt to unify the work programme into a single dependency diagram showing the top-level outputs on the left and contributory work packages to the right.

> The arrows represent dependency relations; so A-->B means that B is a dependency of A. Please feed back to Ashley any changes needed.

```mermaid
graph LR

    subgraph External Deliverables
        A[Publication of 25/26 NHS Payment Scheme]
        AD[Supplementary Payment Guidance]
    end 

    A[Publication of NHS Payment Scheme] -- Depends on --> B[Price Production]

    
    B[Price Production] --> C[High Cost Exclusions]
    B[Price Production] --> D[Low Value Activity]
    B[Price Production] --> E[Cost Uplift Factor]
    B[Price Production] --> F[Clinical Review of Prices]

    A[Publication of NHS Payment Scheme] --> I[S114 Consultation Document]

    I[S114 Consultation] --> F[Clinical Review of Prices] 
    I[S114 Consultation] --> J[Sector Engagement]
    I[S114 Consultation] --> K[EHIA]
    I[S114 Consultation] --> N[Impact Assessment]
       
    A[Publication of NHS Payment Scheme] --> G[Casemix Design]

    G[Casemix Design] --> H[Market Forces Factor]
    G[Casemix Design] --> L[Complexity Analysis]
    G[Casemix Design] --> M[Coding & data quality]

    AD[Supplementary Payment Guidance] --> AE[Fixed Payment Review]
    AD[Supplementary Payment Guidance] --> AF[Elective Prices incl. IS]
    AD[Supplementary Payment Guidance] --> AG[Independent Sector Reimbursement]
    AD[Supplementary Payment Guidance] --> AH[ERF]



    subgraph Internal Deliverables
        O[Proposals for 26/27 NHS Payment Scheme]
        Y[Programme Administration]
    end

    O[Proposals for 26/27 NHS Payment Scheme] --> P[Specialised Commissioning]
    O[Proposals for 26/27 NHS Payment Scheme] --> Q[Mental Health Services Currency Models]
    O[Proposals for 26/27 NHS Payment Scheme] --> R[Community Services Currency Models]
    O[Proposals for 26/27 NHS Payment Scheme] --> S[Products to Support API]
    O[Proposals for 26/27 NHS Payment Scheme] --> T[Future Payment Design]
    O[Proposals for 26/27 NHS Payment Scheme] --> U[Financial Incentives]

    U[Financial Incentives] --> V[Review of BPTs]
    U[Financial Incentives] --> W[CQUIN Review]
    U[Financial Incentives] --> X[System Financial Incentives]

    Y[Programme Administration] --> Z[Pricing Mailbox]
    Y[Programme Administration] --> AA[Programme Management]
    Y[Programme Administration] --> AB[Line Management]
    Y[Programme Administration] --> AC[Team Meetings]
    
    
    
```

Things yet to be categorised

```mermaid
graph LR
    A[Community Diagnostic Centres]
    B[Excess bed day trim points]
```