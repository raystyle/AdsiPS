# AdsiPS

PowerShell module to interact with Active Directory using ADSI and DirectoryServices (.NET)

#### Goals
 * No ActiveDirectory module/No Quest AD Snapin required
 * Being able to specify different credentials
 * Being able to specify different domain
 * If possible avoid use of C# code
  

#### Use Cases

 * Sometime ActiveDirectory Module is not available/ or can't install it on a machine
 * AD queries need to be performed by a tool (GUI for example) and you don't want it to load AD module. Additionally you don't know who will use the tool and if they have/can/know how to install the module.
 * Performance, ADSI is way faster...
 * I can't see the code behind AD Module and Quest AD Snapin, so this is a good way to learn how Active Directory is working

# Installation
To install in your personal modules folder (e.g. ~\Documents\WindowsPowerShell\Modules), run:

```powershell
iex (new-object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/lazywinadmin/AdsiPS/master/install.ps1')
```

# Cmdlets
* Add-ADSIGroupMember
* Enable-ADSIReplicaGC
* Get-ADSIComputer
* Get-ADSIContact
* Get-ADSICurrentComputerSite
* Get-ADSIDomain
* Get-ADSIDomainController
* Get-ADSIDomainDomainControllers
* Get-ADSIDomainMode
* Get-ADSIDomainRoot
* Get-ADSIDomainTrustRelationship
* Get-ADSIForest
* Get-ADSIForestDomain
* Get-ADSIForestMode
* Get-ADSIForestTrustRelationship
* Get-ADSIFsmo
* Get-ADSIGlobalCatalogs
* Get-ADSIGroup
* Get-ADSIGroupManagedBy
* Get-ADSIGroupMembership
* Get-ADSIGroupPolicyObject
* Get-ADSIObject
* Get-ADSIOrganizationalUnit
* Get-ADSIReplicaCurrentTime
* Get-ADSIReplicaDomainInfo
* Get-ADSIReplicaForestInfo
* Get-ADSIReplicaGCInfo
* Get-ADSIReplicaInfo
* Get-ADSISchema
* Get-ADSISite
* Get-ADSISiteConnection
* Get-ADSISiteLink
* Get-ADSISiteServer
* Get-ADSISitesInfo
* Get-ADSITokenGroup
* Get-ADSITrustRelationShip
* Get-ADSIUser
* Move-ADSIDomainControllerRoles
* Move-ADSIReplicaToSite
* New-ADSIDirectoryContextDomain
* New-ADSIDirectoryContextForest
* New-ADSIPrincipalContext
* Remove-ADSIGroupMember
* Start-ADSIReplicationConsistencyCheck
* Test-ADSICredential
* Test-ADSIUserIsGroupMember



# Change Log

# Examples



# To Do
- [x] Add-ADSIGroupMember
- [ ] Add-ADSISiteSubnet
- [ ] Disable-ADSIAccount
- [ ] Enable-ADSIAccount
- [x] Get-ADSIComputer
 - [ ] Param: OperatingSystem
 - [ ] Param: Disabled
- [x] Get-ADSIContact
- [ ] Get-ADSICurrentComputerSite
 - [ ] Comment Based Help
 - [ ] Add Credential
- [x] Get-ADSIDomain
- [x] Get-ADSIDomainController (ADSI)
 - Might get rid of this function
- [x] Get-ADSIDomainDomainControllers (DirectoryServices)
 - [ ] Comment Based Help
- [x] Get-ADSIDomainMode
 - [ ] Comment Based Help
- [x] Get-ADSIDomainTrustRelationship
 - [ ] Comment Based Help
- [x] Get-ADSIForest
- [x] Get-ADSIForestMode
 - [ ] Comment Based Help
- [x] Get-ADSIForestDomain
 - [ ] Comment Based Help
- [x] Get-ADSIForestTrustRelationship
 - [ ] Comment Based Help
- [x] Get-ADSIFsmo
- [x] Get-ADSIGlobalCatalogs
 - [ ] Comment Based Help
- [x] Get-ADSIGroup
 -  [ ] Param: GroupScope (Domain Local, Global, Universal)
 -  [ ] Param: GroupType (Distribution/Security)
 -  [ ] Modify queries to use Anr (Ambiguous Name Resolution)
- [x] Get-ADSIGroupManagedBy
- [x] Get-ADSIGroupMembership
 - [ ] Indirect Members (Check in Chain)
- [x] Get-ADSIGroupPolicyObject
- [x] Get-ADSIObject
- [x] Get-ADSIOrganizationalUnit
- [ ] Get-ADSIPrinterQueue
- [x] Get-ADSIRootDomain
- [ ] Get-ADSIRootDSE
- [x] Get-ADSISchema
- [ ] Get-ADSIServiceAccount
- [x] Get-ADSISite
- [x] Get-ADSISiteConnection
- [x] Get-ADSISiteLink
- [x] Get-ADSISiteServer
- [ ] Get-ADSISiteSubnet
- [x] Get-ADSITrustRelationship
- [x] Get-ADSIUser
 - [ ] Modify queries to use Anr (Ambiguous Name Resolution)
 - [ ] Param: Disabled Account 
 - [ ] Param: Change Password next logon enabled
 - [ ] Param: LockedOut
 - [ ] Param: Disabled
- [ ] Get-ADSIUserResultantPasswordPolicy
- [ ] Lock-ADSIAccount
- [x] New-ADSIDirectoryContextDomain
- [x] New-ADSIDirectoryContextForest
- [ ] New-ADSISite
- [ ] New-ADSIComputer
- [ ] New-ADSIContact
- [ ] New-ADSIDomainTrustRelationship
- [ ] New-ADSIForestTrustRelationship
- [ ] New-ADSIUser
- [ ] New-ADSIGroup
- [ ] New-ADSIOrganizationalUnit
- [ ] Move-ADSIObject
- [x] Remove-ADSIGroupMember
- [ ] Remove-ADSIUser
- [ ] Remove-ADSIComputer
- [ ] Remove-ADSIContact
- [ ] Remove-ADSIDomainTrustRelationship
- [ ] Remove-ADSIOrganizationUnit
- [ ] Remove-ADSIForestTrustRelationship
- [ ] Set-ADSIUser
- [ ] Set-ADSIComputer
- [ ] Set-ADSIContact
- [ ] Set-ADSIGroup
- [ ] Set-ADSIDeletionProtection
- [x] Test-ADSIUserIsGroupMember
- [ ] Unlock-ADSIAccount
- AdsiPS replication cmdlets
- [x] Get-ADSIReplicaInfo
- [x] Get-ADSIReplicaForestInfo
- [x] Get-ADSIReplicaDomainInfo
- [x] Get-ADSIReplicaCurrentTime
- [x] Get-ADSIReplicaGCInfo
- [x] Enable-ADSIReplicaGC
- [x] Get-ADSISitesInfo
- [x] Move-ADSIDomainControllerRoles
- [x] Move-ADSIReplicaToSite
- [x] Start-ADSIReplicationConsistencyCheck
