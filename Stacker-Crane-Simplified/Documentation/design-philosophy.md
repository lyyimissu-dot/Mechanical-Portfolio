# Design Philosophy

The simplified model follows real engineering principles used in industrial storage automation.

## 1. Load Path Orientation
The mast carries vertical loads and resists bending caused by fork extension.  
The base frame transfers horizontal forces into the floor rails.

## 2. Stiffness Before Strength
Stacker cranes typically fail by **excessive deflection**, not material failure.  
Therefore, stiffness (EI) is the primary design criterion.

## 3. Simplification Strategy
To protect proprietary details, the real design is replaced with:
- Beam representations for forks and masts  
- Rigid blocks representing the carriage and platform  
- Generic weldments instead of detailed joints  

## 4. Safety Philosophy
- Redundant limit switches  
- Overtravel prevention  
- Load stability margin  
- Torque limits for servos  

The design philosophy provides the foundation for the simplified analysis in this repository.
