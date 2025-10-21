# 5. Mass User Creation — SU10

The `SU10` transaction allows batch operations for multiple users simultaneously.

## 1️⃣ Access the Transaction  
`/nSU10`

## 2️⃣ Select Users  
- Enter user IDs manually or use **Multiple Selection**.  
- Optionally, import from file (`Ctrl + F11 → Upload from file`).

## 3️⃣ Available Actions
| Action | Description |
|--------|-------------|
| Change | Modify user data in bulk |
| Lock/Unlock | Mass lock/unlock users |
| Assign Roles | Add roles to multiple users |
| Delete Roles | Remove roles |
| Set Password | Reset initial passwords |

## 4️⃣ Mass Creation via Reference User  
- Copy from reference user: `User → Copy From → Reference User`  
- Adjust address, validity, and role assignments.  
- Run **User Comparison (F8)**.

## 5️⃣ Logging & Audit  
Use `SUIM → Change Documents for Users` to review mass changes.  
Export logs for compliance verification.

## 6️⃣ GRC AC Integration (optional)  
If **SAP GRC Access Control** is implemented:  
- Use **Access Request Management (ARM)** workflow  
- Approvals configured in **BRF+**  
- Automatic provisioning via RFC connection to target system
