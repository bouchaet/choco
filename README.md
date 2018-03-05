# quick setup with chocolatey
Simple scripts to install packages to setup a development environment with choco (windows)

## prerequisites
* choco  
You can install [choco](https://chocolatey.org/docs/installation#install-with-cmdexe) from a command prompt with:  
`@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`
* curl  
Curl can be installed with choco (see [gallery](https://chocolatey.org/packages/curl)): `choco install curl`

## install
Enable global confirmation (optional but otherwise you will be prompted for confirmation)  
`> choco feature enable -n allowGlobalConfirmation`

From a command prompt:  
`> curl -sSL https://raw.githubusercontent.com/bouchaet/choco/master/setupdev | cmd`  
  
For more languages (erlang, rust, ...) and docker + minikube, use:  
`> curl -sSL https://raw.githubusercontent.com/bouchaet/choco/master/setupdev-full | cmd`  
