## [NEX-Protocols](https://github.com/kinnay/NintendoClients/wiki/NEX-Protocols) > AccountManagementProtocol (Unknown ID)

| Method ID | Method Name |
| --- | --- |
| 1 | [CreateAccount](#1-createaccount) |
| 2 | [DeleteAccount](#2-deleteaccount) |
| 3 | [DisableAccount](#3-disableaccount) |
| 4 | [ChangePassword](#4-changepassword) |
| 5 | [TestCapability](#5-testcapability) |
| 6 | [GetName](#6-getname) |
| 7 | [GetAccountData](#7-getaccountdata) |
| 8 | [GetPrivateData](#8-getprivatedata) |
| 9 | [GetPublicData](#9-getpublicdata) |
| 10 | [GetMultiplePublicData](#10-getmultiplepublicdata) |
| 11 | [UpdateAccountName](#11-updateaccountname) |
| 12 | [UpdateAccountEmail](#12-updateaccountemail) |
| 13 | [UpdateCustomData](#13-updatecustomdata) |
| 14 | [FindByNameRegex](#14-findbynameregex) |
| 15 | [UpdateAccountExpiryDate](#15-updateaccountexpirydate) |
| 16 | [UpdateAccountEffectiveDate](#16-updateaccounteffectivedate) |
| 17 | [UpdateStatus](#17-updatestatus) |
| 18 | [GetStatus](#18-getstatus) |
| 19 | [GetLastConnectionStats](#19-getlastconnectionstats) |
| 20 | [ResetPassword](#20-resetpassword) |
| 21 | [CreateAccountWithCustomData](#21-createaccountwithcustomdata) |
| 22 | [RetrieveAccount](#22-retrieveaccount) |
| 23 | [UpdateAccount](#23-updateaccount) |
| 24 | [ChangePasswordByGuest](#24-changepasswordbyguest) |
| 25 | [FindByNameLike](#25-findbynamelike) |
| 26 | [CustomCreateAccount](#26-customcreateaccount) |
| 27 | [NintendoCreateAccount](#27-nintendocreateaccount) |
| 28 | [LookupOrCreateAccount](#28-lookuporcreateaccount) |
| 29 | [DisconnectPrincipal](#29-disconnectprincipal) |
| 30 | [DisconnectAllPrincipals](#30-disconnectallprincipals) |

# (1) CreateAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strPrincipalName |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |

# (2) DeleteAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |

## Response
This method does not return anything

# (3) DisableAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | dtUntil |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strMessage |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |

# (4) ChangePassword

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strNewKey |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |

# (5) TestCapability

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | uiCapability |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |

# (6) GetName

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strName |  |

# (7) GetAccountData

## Request
This method does not take any parameters

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| [AccountData](#accountdata-structure) | oAccountData |  |

# (8) GetPrivateData

## Request
This method does not take any parameters

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oData |  |

# (9) GetPublicData

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oData |  |

# (10) GetMultiplePublicData

## Request
| Type | Name | Description |
| --- | --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;Uint32&#x3E; | lstPrincipals |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;any&#x3E; | oData |  |

# (11) UpdateAccountName

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strName |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |

# (12) UpdateAccountEmail

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strName |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |

# (13) UpdateCustomData

## Request
| Type | Name | Description |
| --- | --- | --- |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPublicData |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPrivateData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |

# (14) FindByNameRegex

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strRegex |  |
| [ResultRange](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#resultrange) | resultRange |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[BasicAccountInfo](#basicaccountinfo-structure)&#x3E; | plstAccounts |  |

# (15) UpdateAccountExpiryDate

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | dtExpiry |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strExpiredMessage |  |

## Response
This method does not return anything

# (16) UpdateAccountEffectiveDate

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | dtEffectiveFrom |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strNotEffectiveMessage |  |

## Response
This method does not return anything

# (17) UpdateStatus

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strStatus |  |

## Response
This method does not return anything

# (18) GetStatus

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strStatus |  |

# (19) GetLastConnectionStats

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | dtLastSessionLogin |  |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | dtLastSessionLogout |  |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | dtCurrentSessionLogin |  |

# (20) ResetPassword

## Request
This method does not take any parameters

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |

# (21) CreateAccountWithCustomData

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strPrincipalName |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPublicData |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPrivateData |  |

## Response
This method does not return anything

# (22) RetrieveAccount

## Request
This method does not take any parameters

## Response
| Type | Name | Description |
| --- | --- | --- |
| [AccountData](#accountdata-structure) | oAccountData |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPublicData |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPrivateData |  |

# (23) UpdateAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPublicData |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oPrivateData |  |

## Response
This method does not return anything

# (24) ChangePasswordByGuest

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strPrincipalName |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |

## Response
This method does not return anything

# (25) FindByNameLike

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strLike |  |
| [ResultRange](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#resultrange) | resultRange |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[BasicAccountInfo](#basicaccountinfo-structure)&#x3E; | plstAccounts |  |

# (26) CustomCreateAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strPrincipalName |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oAuthData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | pid |  |

# (27) NintendoCreateAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strPrincipalName |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oAuthData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | pid |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | pidHMAC |  |

# (28) LookupOrCreateAccount

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strPrincipalName |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strKey |  |
| Uint32 | uiGroups |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strEmail |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oAuthData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | pid |  |

# (29) DisconnectPrincipal

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idPrincipal |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |

# (30) DisconnectAllPrincipals

## Request
This method does not take any parameters

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |

# Types

## AccountData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_pid |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strName |
| Uint32 | m_uiGroups |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strEmail |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | m_dtCreationDate |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | m_dtEffectiveDate |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strNotEffectiveMsg |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | m_dtExpiryDate |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strExpiredMsg |

## BasicAccountInfo ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_pidOwner |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strName |

## PublicData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

This structure does not contain any fields.

## PrivateData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

This structure does not contain any fields.