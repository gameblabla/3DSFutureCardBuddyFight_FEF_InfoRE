## [NEX-Protocols](https://github.com/kinnay/NintendoClients/wiki/NEX-Protocols) > TicketGrantingProtocol (Unknown ID)

| Method ID | Method Name |
| --- | --- |
| 1 | [Login](#1-login) |
| 2 | [LoginEx](#2-loginex) |
| 3 | [RequestTicket](#3-requestticket) |
| 4 | [GetPID](#4-getpid) |
| 5 | [GetName](#5-getname) |
| 6 | [LoginWithContext](#6-loginwithcontext) |

# (1) Login

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strUserName |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| Uint32 | pidPrincipal |  |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | pbufResponse |  |
| [RVConnectionData](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#rvconnectiondata) | pConnectionData |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strReturnMsg |  |

# (2) LoginEx

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strUserName |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | oExtraData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| Uint32 | pidPrincipal |  |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | pbufResponse |  |
| [RVConnectionData](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#rvconnectiondata) | pConnectionData |  |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strReturnMsg |  |

# (3) RequestTicket

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | idSource |  |
| Uint32 | idTarget |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | bufResponse |  |

# (4) GetPID

## Request
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | strUserName |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | %retval% |  |

# (5) GetName

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | id |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | %retval% |  |

# (6) LoginWithContext

## Request
| Type | Name | Description |
| --- | --- | --- |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | loginData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| Uint32 | pidPrincipal |  |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | pbufResponse |  |
| [RVConnectionData](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#rvconnectiondata) | pConnectionData |  |

# Types

## RVConnectionData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | m_urlRegularProtocols |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;Uint8&#x3E; | m_lstSpecialProtocols |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | m_urlSpecialProtocols |
| __dummy_revision | __dummy_revision1 |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | m_currentUTCTime |

## LoginData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Sint8 | m_principalType |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_userName |
| Uint64 | m_context |
| Uint32 | m_similarConnection |