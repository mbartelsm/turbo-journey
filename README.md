# turbo-journey

## Goal

Make a tool that will procedurally generate a list of fictional rulers with associated data.

List view:
```
...
Ocander Iliros (63 IR - 138 IR)...
Mandor Ameran (103 IR - 151 IR), ruled 138 IR - 151 IR.
Mandoris Ameran (124 IR - 154 IR)...
...
```
Ruler view
```
Mandor Ameran (103 IR - 151 IR)
  Offices held:
  | General of the Yulas Army: 127 IR - 129 IR
  | Ambassador of the Yulas Clan to the Empire: 129 IR - 132 IR
  | Chief of the Yulas Clan: 132 IR - 138 IR
  | Emperor of the Angaran Empire: 138 IR - 146 IR.
  | Co-emperor of the Angaran Empire: 146 IR - 151 IR
  
  Deeds:
  | Defeat of the Tamargis clan Army
  | Establishment of a progressive economic policy
```

## Implementation

For starters, only the List view will be implemented.

### Names

Names will be generated either using a markov chain, a constrained randomized string, or a premade list of approved names. Names of important rulers are more likely to be repeated as is or with variations. Importance can be measured as a factor of rule length or other variables later implemented.

### Rule length

Defined

Each ruler leaves a footprint in the empire, a bad ruler will leave a negative footprint, making it more likely for usurpation to occur to himself and future rulers. The more negative the footprint, the better an emperor needs to be to survive. 
