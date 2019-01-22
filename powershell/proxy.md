# Get things to work behind the proxy

    PS >  [System.Net.WebRequest]::DefaultWebProxy.Credentials = [System.Net.CredentialCache]::DefaultCredentials

Also need to register the repository:

    PS > Register-PSRepository -Name PSGallery -SourceLocation https://www.powershellgallery.com/api/v2
