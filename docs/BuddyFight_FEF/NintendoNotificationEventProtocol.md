## [NEX-Protocols](https://github.com/kinnay/NintendoClients/wiki/NEX-Protocols) > NintendoNotificationEventProtocol (Unknown ID)

| Method ID | Method Name |
| --- | --- |
| 1 | [ProcessNintendoNotificationEvent](#1-processnintendonotificationevent) |

# (1) ProcessNintendoNotificationEvent

## Request
| Type | Name | Description |
| --- | --- | --- |
| [NintendoNotificationEvent](#nintendonotificationevent-structure) | oEvent |  |

## Response
This method does not return anything

# Types

## u8KeyValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint8 | m_key |
| Uint8 | m_value |

## u32KeyValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint8 | m_key |
| Uint32 | m_value |

## u64KeyValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint8 | m_key |
| Uint64 | m_value |

## StringKeyValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint8 | m_key |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_value |

## GameKey ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint64 | m_gameCode |
| Uint16 | m_gameVersion |

## NintendoNotificationEvent ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_uiType |
| Uint32 | m_pidSender |
| [AnyDataHolder](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#anydataholder) | m_dataholder |

## NintendoNotificationEventGeneral ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint32 | m_u32Param |
| Uint64 | m_u64Param1 |
| Uint64 | m_u64Param2 |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strParam |

## NintendoNotificationEventKeyValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[u8KeyValue](#u8keyvalue-structure)&#x3E; | m_lstu8Param |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[u32KeyValue](#u32keyvalue-structure)&#x3E; | m_lstu32Param |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[u64KeyValue](#u64keyvalue-structure)&#x3E; | m_lstu64Param |
| [List](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#list)&#x3C;[StringKeyValue](#stringkeyvalue-structure)&#x3E; | m_lststrParam |

## NintendoNotificationEventProfile ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint8 | m_region |
| Uint8 | m_country |
| Uint8 | m_area |
| Uint8 | m_language |
| Uint8 | m_platform |

## NintendoPresence ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#data)

| Type | Name |
| --- | --- |
| Uint32 | m_changedBitFlag |
| [GameKey](#gamekey-structure) | m_gameKey |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_gameModeDescription |
| Uint32 | m_joinAvailabilityFlag |
| Uint8 | m_matchmakeSystemType |
| Uint32 | m_joinGameID |
| Uint32 | m_joinGameMode |
| Uint32 | m_ownerPrincipalID |
| Uint32 | m_joinGroupID |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | m_applicationArg |