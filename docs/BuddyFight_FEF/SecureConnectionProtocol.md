## [NEX-Protocols](https://github.com/kinnay/NintendoClients/wiki/NEX-Protocols) > SecureConnectionProtocol (Unknown ID)

| Method ID | Method Name |
| --- | --- |
| 1 | [Register](#1-register) |
| 2 | [RequestConnectionData](#2-requestconnectiondata) |
| 3 | [RequestURLs](#3-requesturls) |
| 4 | [RegisterEx](#4-registerex) |
| 5 | [TestConnectivity](#5-testconnectivity) |
| 6 | [UpdateURLs](#6-updateurls) |
| 7 | [ReplaceURL](#7-replaceurl) |
| 8 | [SendReport](#8-sendreport) |

# (1) Register

## Request
| Type | Name | Description |
| --- | --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl)&#x3E; | vecMyURLs |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| Uint32 | pidConnectionID |  |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | urlPublic |  |

# (2) RequestConnectionData

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | cidTarget |  |
| Uint32 | pidTarget |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[ConnectionData](#connectiondata-structure)&#x3E; | pvecConnectionsData |  |

# (3) RequestURLs

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | cidTarget |  |
| Uint32 | pidTarget |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| Bool | %retval% |  |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl)&#x3E; | plstURLs |  |

# (4) RegisterEx

## Request
| Type | Name | Description |
| --- | --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl)&#x3E; | vecMyURLs |  |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | hCustomData |  |

## Response
| Type | Name | Description |
| --- | --- | --- |
| [Result](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#result) | %retval% |  |
| Uint32 | pidConnectionID |  |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | urlPublic |  |

# (5) TestConnectivity

## Request
This method does not take any parameters

## Response
This method does not return anything

# (6) UpdateURLs

## Request
| Type | Name | Description |
| --- | --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl)&#x3E; | vecMyURLs |  |

## Response
This method does not return anything

# (7) ReplaceURL

## Request
| Type | Name | Description |
| --- | --- | --- |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | target |  |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | url |  |

## Response
This method does not return anything

# (8) SendReport

## Request
| Type | Name | Description |
| --- | --- | --- |
| Uint32 | reportId |  |
| [qBuffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#qbuffer) | reportData |  |

## Response
This method does not return anything

# Types

## ConnectionData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| [StationURL](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#stationurl) | m_StationUrl |
| Uint32 | m_ConnectionID |