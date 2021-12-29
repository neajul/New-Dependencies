# temporary/permanent
```mermaid
sequenceDiagram
    participant Homeless
    participant Squat
    participant Woongroep
    Homeless->>Squat: occupation
    Note over Squat: temporary
    Note over Woongroep: permanent
    Squat->>Homeless: eviction
    Squat-->>Woongroep: legalization
```
# impermanence
```mermaid
graph TD;
		A[/no place to be\];
		B[(squat)];
		C[\no longer a squat/];
    A-- squatting -->B;
    B-- eviction -->A;
    B-- legalization -->C;
```

# Mokum Journey 2

```mermaid
flowchart LR;
		1[(Joes Garage)];
		2[(Bowling)];
		3[(Kinderen van Mokum)];
		4[(Villa Ivivke)];
		5[(Hotel Mokum)];
		
    A[angry individuals];
    B([meetings]);
    C[action group];
    
    subgraph planning;
    		A-->B-->C;
    end;
    1-- facilitated -->planning;
    2-- facilitated -->planning;
    
    D[action group];
    E([squats]);
    F[Hotel Marnix];
    
    subgraph action;
    		D-->E-->F;
    end;
    action --> 5;
    1-- advised -->action;
    2-- supplied materials -->action;
    
    G[abandoned building];
    H([renovation]);
    I[public events];
    
    subgraph occupation;
    		G-->H-->I;
    end;
    3-- plumbing, floors -->occupation;
    4-- electricity -->occupation;
    
    J[municipality]
    K([evicts])
    L[angry individuals]
    
    subgraph eviction
    		J-->K-->L
    end
    1 & 2 & 3 --> eviction
    
    planning-->action;
    action-->occupation;
    occupation-->eviction;
```
