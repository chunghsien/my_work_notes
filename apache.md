LoadModule fcgid_module modules/mod_fcgid.so
FcgidInitialEnv PHPRC "C:\php\php-5.6.39-nts"
FcgidInitialEnv PATH "C:\php\php-5.6.39-nts;C:/WINDOWS/system32;C:/WINDOWS;C:/WINDOWS/System32/Wbem;"
FcgidInitialEnv SystemRoot "C:/Windows"
FcgidInitialEnv SystemDrive "C:"
FcgidInitialEnv TEMP "C:/WINDOWS/Temp"
FcgidInitialEnv TMP "C:/WINDOWS/Temp"
FcgidInitialEnv windir "C:/WINDOWS"
FcgidIOTimeout 64
FcgidConnectTimeout 16
FcgidMaxRequestsPerProcess 500
MaxRequestLen 1000000000000

<Files ~ "\.php$">
    Options Indexes FollowSymLinks ExecCGI
    AddHandler fcgid-script .php
    FcgidWrapper "C:/php/php-5.6.39-nts/php-cgi.exe" .php	
</Files>

SetOutputFilter DEFLATE
AddOutputFilterByType DEFLATE text/html text/plain text/xml text/css text/javascript application/x-javascript application/javascript application/json image/jpeg
AddOutputFilter DEFLATE js css svg png gif jpg jpeg
DeflateCompressionLevel 6 
