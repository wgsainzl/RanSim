 <#

.SYNOPSIS
    Ransomware Simulator using AES to recursively encrypt or decrypt files at a given path

.DESCRIPTION
    This script is intended to be used to test your defenses and backups against ransomware in a controlled environment. You can encrypt fake data for
your simulation, but you also have the option to decrypt the files with the same script if you need to.

.EXAMPLE
    .\RanSim.ps1 -mode encrypt
    or
    .\RanSim.ps1 -mode decrypt

.PARAMETER Target File Path
    This optional parameter specifies the path that the recursive encryption will start in. A default path is provided.
 
.PARAMETER File Extension
    This optional parameter defines the extension that will be added to the encrypted files once attacked. A default extension is provided.

.PARAMETER Encryption key
    This optional parameter is the plain-text AES encryption key used for both encryption and decryption. A default key is provided. 

.NOTES
    This script uses the FileCryptopgraphy module from Tyler Siegrist - https://gallery.technet.microsoft.com/scriptcenter/EncryptDecrypt-files-use-65e7ae5d

#>
