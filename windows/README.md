Disable tips, tricks, and suggestions

```powershell
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\ContentDeliveryManager" -Name "SoftLandingEnabled" -Value 0 -Force
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\ContentDeliveryManager" -Name "SubscribedContent-338389Enabled" -Value 0 -Force
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\ContentDeliveryManager" -Name "SubscribedContent-338393Enabled" -Value 0 -Force
```

Update with winget and Windows store
```powershell
winget upgrade --all
store updates
```

Set up Windows 11 without internet

Open cmd with Shift + F10
```cmd
oobe\bypassnro
```

Create a new account
Note: Use "" if you have spaces in the account name

```powershell
net user account_name new_password /add
```

Change account to admin
Note: If the system has English locale use Administrator

```
net localgroup Administratörer admin /add
```

# Windows Run Commands (Win + R)

# System Tools

## Device Manager
devmgmt.msc

## Group Policy Editor
gpedit.msc

## Local Users and Groups
lusrmgr.msc
