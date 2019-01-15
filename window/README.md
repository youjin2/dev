# Window Settings
* File size limit between local and web  
(https://extrememanual.net/327)
    - open regedit (window + R)
    - go to  
    `컴퓨터\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\WebClient\Parameters`
    - change `FileSizeLimitInBytes` value data to 4000000000 (decimal number)
