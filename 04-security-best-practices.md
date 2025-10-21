# 4. Security Best Practices

## 1️⃣ Segregation of Duties (SoD)
Avoid assigning conflicting functions to the same user (e.g., create and approve payment).

Tooling:  
- **GRC Access Control (A.C. 12.0+)**  
- Risk analysis via `GRAC_SOD` or `NWBC → Access Risk Analysis`

## 2️⃣ Naming Policy
| User Type | Format Example | Description |
|------------|----------------|-------------|
| Dialog | `FIRST.LAST` | Real user accounts |
| Technical | `ZSYS_<DESC>` | Background/system users |
| Test | `ZTST_<DESC>` | Sandbox/testing users |

## 3️⃣ Licensing Compliance
- Regularly review **USMM** and **SLAW2**  
- Ensure correct **User Type** (Dialog, System, etc.)

## 4️⃣ Auditing
- Track user changes via `SUIM → Change Documents for Users`  
- Enable **Security Audit Log** in `SM19/SM20` for sensitive users

## 5️⃣ Inactive User Policy
Lock or delete users inactive for >90 days:  
`SU10 → Lock Users`

## 6️⃣ Backup and Export
Export user and role lists for review:  
`SUIM → Users by Complex Selection Criteria`  
`System → List → Export → Spreadsheet`
