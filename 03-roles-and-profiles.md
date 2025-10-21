# 3. Roles and Profiles

## Concepts

| Concept | Description |
|----------|-------------|
| Role (PFCG Role) | Logical collection of transactions, objects, and authorizations |
| Profile | Technical object generated from a role |
| Composite Role | Group of multiple single roles |

## Creating a Role
1. Access `/nPFCG`  
2. Enter role name (e.g., `Z_SD_SALES_REP`)  
3. Fill in:  
   - Description  
   - Menu (transactions)  
   - Authorizations  
   - Users  
4. Click **Generate (Profile → Save)**

## Role Comparison
Use transaction `SUPC` to regenerate profiles in bulk.

## Role Assignment
- Always assign roles via **Roles** tab in `SU01`.  
- After role updates, execute **User Comparison (F8)**.

## Best Practices
- Never use wildcard authorizations (`*`).  
- Separate roles by access type (Display / Change).  
- Apply naming conventions:  
  `Z_<Module>_<Function>_<Type>`  
  Example: `Z_MM_PURCH_REQ_DISPLAY`
