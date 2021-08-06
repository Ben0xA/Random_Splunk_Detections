```
index=main EventCode=5145 Access_Mask="0x3"
| regex Relative_Target_Name="(?i)((lsa|efs)rpc|lsass|netlogon)"
| regex Accesses="(?i)((read|write)data|addfile)"
| table _time, host, Account_Name, Account_Domain, Source_Address, Share_Name, Relative_Target_Name
| sort -_time
```
