# Structural Patterns in Organizational Graphs

This document describes common patterns found in organizational structures that can indicate potential issues with transparency, efficiency, or corruption risks.

## 1. Opaque Intermediary

**Description**: Information flows through a middle manager without direct access to higher authority. The intermediary can distort or filter information.

**Pattern**:
```
A → B → C
```

## 2. Responsibility Overload

**Description**: A single person has too many direct reports, reducing the ability to manage effectively.

**Pattern**:
```
X1 → Manager
X2 → Manager
...
X8 → Manager
```

## 3. Conflicted Subordination

**Description**: One employee reports to multiple managers who are not aligned in a clear hierarchy. This leads to task conflicts, overlapping expectations, and a lack of unified responsibility for decision-making.

**Pattern**:
```
A → B
A → C
A → D
```

## 4. Isolated Node

**Description**: An individual is not connected to the organizational graph, leading to exclusion from communication and control.

**Pattern**:
```
(no edges)
```

## 5. Cross-Level Skip

**Description**: Someone reports directly to a much higher level, skipping layers of management and reducing structure clarity.

**Pattern**:
```
A → D (where B and C are skipped)
```

## 6. Circular Delegation

**Description**: A closed loop of responsibilities, which can obscure accountability.

**Pattern**:
```
A → B → C → A
```

## 7. Single Gatekeeper

**Description**: A single node controls access to other parts of the organization, creating a bottleneck or potential abuse point.

**Pattern**:
```
A → Gatekeeper → B
```

## 8. Asymmetric Burden

**Description**: Managers have vastly different numbers of subordinates, indicating unbalanced distribution of responsibility.

**Pattern**:
```
X1-X4 → M1
Y1 → M2
```

## 9. Information Monoculture

**Description**: All inputs come from a similar group or role, creating a lack of diversity in feedback.

**Pattern**:
```
E1 → M
E2 → M
E3 → M
E4 → M
```

## 10. Phantom Node

**Description**: A node that appears in the graph but has no meaningful function or connection in actual operations.

**Pattern**:
```
A → Phantom
B → Phantom
C → Phantom
```
