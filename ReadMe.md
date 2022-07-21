# Client certificate auth dotnet 6

Original repo from here:


https://github.com/niteshsinghal85/blogs/tree/main/CertificateAuthExample




Issue with kestrel  on RHEL 9
Configuration doesn't work as requried here:

https://docs.microsoft.com/en-us/aspnet/core/security/authentication/certauth?view=aspnetcore-6.0#configure-your-server-to-require-certificates



Clean dev cert first:


          dotnet dev-certs https --clean


Generate cert:


        dotnet dev-certs https  -ep dev_cert.pfx -p 12345
