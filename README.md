# ElevateLabs_CS_Task07
Identify and Remove Suspicious Browser Extensions
# Suspicious Extensions Removed

Date: 2025-10-03
Browser: Google Chrome (Version ...)

## Removed items
1. **Ad Cleaner Pro** (id: abcdefghijklmnop)
   - Why: Requests "Read and change all your data on all websites", very low installs, name imitates legitimate adblockers, update_url points to non-store host.
   - Evidence: screenshots/ad_cleaner_pro_details.png
   - Action: Disabled then Removed via chrome://extensions. Confirmed removed and Chrome restarted.

2. **NewTab XYZ** (id: zyxwvutsrqponm)
   - Why: Injected new tab redirect to suspicious search engine; high CPU usage in Chrome Task Manager.
   - Evidence: screenshots/newtab_xyz_taskmgr.png
   - Action: Removed. Also deleted registry entry in HKCU:\Software\Google\Chrome\Extensions\<id>.

## Post-cleanup
- Browser restarted, unusual redirects stopped.
- Ran Malwarebytes scan (report: reports/malware_scan.txt) — no additional findings.
