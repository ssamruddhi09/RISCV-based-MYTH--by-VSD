# RISC-V MYTH Workshop — Environment Setup (VSD)

This document records the setup and verification steps for running the RISC-V workshop environment using GitHub Codespaces and the Linux desktop interface.

---

## 1. GitHub Codespace Setup

Opened the RISC-V Codespace using the link provided in the intro mail.

Steps followed:

- Go to repository → **Code**
- Select **Codespaces**
- Click **Create codespace on main**

<img width="1920" height="1200" alt="Codespace Setup" src="https://github.com/user-attachments/assets/abf0ea3c-ed47-42db-b4cd-9e852437a995" />

---

## 2. Verification of Setup

Ran a sample program inside the Codespace to confirm the environment was working correctly.

<img width="1920" height="1200" alt="Verification" src="https://github.com/user-attachments/assets/662fb8f7-85e9-4705-ac10-f18082358693" />

---

## 3. Linux Desktop Setup in Cloud

Opened the Linux desktop interface:

- Navigate to **PORTS** tab
- Click **Follow forwarded address** for the noVNC Desktop port

<img width="1920" height="1200" alt="Linux Desktop Port" src="https://github.com/user-attachments/assets/b784ebb3-f605-4e3c-b688-1a6818804b30" />

---

## 4. Linux Desktop Window

A new browser tab opens showing the Linux GUI environment.

<img width="1920" height="1200" alt="Linux Window" src="https://github.com/user-attachments/assets/4a7ba271-10e2-403f-9f36-d4b2d7bb5607" />

---

## 5. Running Sample Program

Opened terminal inside the Linux desktop and navigated to the sample directory:

```bash
cd /workspaces/vsd-riscv2
cd samples
ls -ltr
```

Compiled and executed a sample program (Native GCC x86):

```bash
gcc sum1ton.c
./a.out
```

<img width="1920" height="1200" alt="Sample Run" src="https://github.com/user-attachments/assets/180d751a-84de-406a-864a-6f2159b37dee" />

---

## 6. Editing Source Code

Opened the source file using the GUI editor:

```bash
gedit sum1ton.c &
```

<img width="1920" height="1200" alt="Editor" src="https://github.com/user-attachments/assets/98613901-f058-4548-9cec-66f3aa652ef8" />

---

## 7. Modifying and Re-running

Modified the value:

```
n = 15
```

Saved the file and recompiled:

```bash
gcc sum1ton.c
./a.out
```

The updated output was displayed in the terminal.

<img width="1920" height="1200" alt="Output" src="https://github.com/user-attachments/assets/99ee48b8-d781-46ca-bd12-5df0351c18fc" />

---

## Result

The Codespace environment, Linux desktop, compiler setup, and execution flow were verified successfully. Sample program compilation and modification worked as expected.

