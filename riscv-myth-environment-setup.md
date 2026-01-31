
You said:
# RISC-V MYTH Workshop — Environment Setup (VSD)

This document records the setup and verification steps for running the RISC-V workshop environment using GitHub Codespaces and the Linux desktop interface.

---

## 1. GitHub Codespace Setup

Opened the RISC-V Codespace using the link provided in the intro mail.

Steps followed:

- Go to repository → **Code**
- Select **Codespaces**
- Click **Create codespace on main**
<img width="1920" height="1200" alt="2" src="https://github.com/user-attachments/assets/c4202e4d-c5cd-4585-a3a1-4dbe57afb2ac" />
 ---
 ## 2. Verification of Setup Ran a sample program inside the Codespace to confirm the environment was working correctly.
<img width="1920" height="1200" alt="3" src="https://github.com/user-attachments/assets/edfcf72c-341b-4e54-b375-24e18df7e72c" />
---
## 3. Linux Desktop Setup in Cloud Opened the Linux desktop interface: - Navigate to **PORTS** tab - Click **Follow forwarded address** for the noVNC Desktop port
<img width="1920" height="1200" alt="4" src="https://github.com/user-attachments/assets/7c4e9b4c-49db-4fc1-b9ff-add273fd6d69" />
---
## 4. Linux Desktop Window A new browser tab opens showing the Linux GUI environment.
<img width="1920" height="1200" alt="5" src="https://github.com/user-attachments/assets/028adb22-24a3-4ba3-8955-aa832a5ef5e0" />
---
## 5. Running Sample Program Opened terminal inside the Linux desktop and navigated to the sample directory:
bash
cd /workspaces/vsd-riscv2
cd samples
ls -ltr
Compiled and executed a sample program (Native GCC x86):
bash
gcc sum1ton.c
./a.out
<img width="1920" height="1200" alt="6" src="https://github.com/user-attachments/assets/7e11fb8f-f162-44e8-82f6-b10fdf4c7ab5" />
---
## 6. Editing Source Code Opened the source file using the GUI editor:
bash
gedit sum1ton.c &
<img width="1920" height="1200" alt="7" src="https://github.com/user-attachments/assets/c687d48d-62d2-422a-872b-1963dd0306de" />
---
## 7. Modifying and Re-running Modified the value:
n = 15
Saved the file and recompiled:
bash
gcc sum1ton.c
./a.out
The updated output was displayed in the terminal.
<img width="1920" height="1200" alt="8" src="https://github.com/user-attachments/assets/580f3646-bf87-4438-8e19-80b8ae3fce39" />
---
