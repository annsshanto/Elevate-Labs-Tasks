# Browser Extension Security Audit

## Objective
Identify and remove potentially harmful browser extensions.

## Environment
- OS: Kali Linux
- Browser: Google Chrome
- Date: 23 Feb 2026

---

## Step 1: Open Extension Manager

URL:
```
chrome://extensions/
```

Screenshot:
![Extensions List](extensions-list.png)

---

## Step 2: Review Installed Extensions

| Extension Name | Developer | Permissions | Suspicious? |
|---------------|-----------|------------|-------------|
| XYZ Tool | Unknown Dev | Read all site data | YES |
| Grammarly | Grammarly Inc | Limited | NO |

---

## Step 3: Suspicious Extension Identified

Extension: XYZ Tool  
Reason:
- Unknown publisher
- Excessive permissions
- Low rating

Screenshot:
![Permissions](extension-permissions.png)

---

## Step 4: Removed Extension

Action:
Removed via extension manager.

Screenshot:
![Removed](extension-removed.png)

---

## Findings

1 suspicious extension removed.

---

## How Malicious Extensions Harm Users

- Data theft
- Credential harvesting
- Session hijacking
- Ad injection
- Browser hijacking

---

## Conclusion

System cleaned and browser performance improved.
