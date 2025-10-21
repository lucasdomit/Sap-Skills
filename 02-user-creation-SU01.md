# 2. User Creation — Transaction SU01

The SAP user creation process must follow standardized governance and security guidelines.

## Step-by-Step Procedure

1️⃣ Access the Transaction  
`/nSU01`

2️⃣ Create a New User  
- Click **Create (F8)**  
- Enter **User ID** following naming conventions (e.g., `L.DOMIT`, `ZUSR001`)

3️⃣ Address Tab  
- **Last Name** / **First Name**  
- **Email**  
- **Language** (`EN`, `PT`, etc.)  
- **Time Zone**

4️⃣ Logon Data Tab  
| Field | Description |
|--------|-------------|
| User Type | `Dialog`, `System`, `Communication`, `Service`, `Reference` |
| Valid From / To | Validity period |
| Initial Password | Temporary password (force change at first logon) |
| SNC | For SSO if applicable |

5️⃣ Roles Tab  
- Assign roles created via transaction `PFCG`  
- Avoid manual profile assignment  
- Define validity period for each role

6️⃣ Parameters Tab  
Add commonly used parameters:  
| Parameter | Value | Description |
|------------|--------|-------------|
| `BUK` | 1000 | Company code |
| `VKO` | 1010 | Sales organization |
| `WRK` | 1100 | Default plant |

7️⃣ Groups Tab  
- Assign **User Group** for segmentation (e.g., `Z_SD`, `Z_MM`, `Z_BASIS`).

8️⃣ License Data Tab  
- Select correct **license type** (e.g., *Professional*, *Employee*)  
- Used for **USMM/SLAW2** license measurement

## Post-Creation Checks
- Log in as the new user and test access.  
- Run `SU53` if an authorization error occurs.  
- Run `SU56` to inspect authorization buffer.
