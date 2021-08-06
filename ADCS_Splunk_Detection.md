```
index=main EventCode=5136 LDAP_Display_Name="userCertificate"
| eval Operation_Type=mvindex(Type,2)
| table _time, host, Account_Name, Account_Domain, Name, LDAP_Display_Name, Operation_Type
| sort -_time
```
