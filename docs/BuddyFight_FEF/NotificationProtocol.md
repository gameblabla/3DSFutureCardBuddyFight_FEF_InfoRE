## [NEX-Protocols](https://github.com/kinnay/NintendoClients/wiki/NEX-Protocols) > NotificationProtocol (Unknown ID)

| Method ID | Method Name |
| --- | --- |
| 1 | [ProcessNotificationEvent](#1-processnotificationevent) |

# (1) ProcessNotificationEvent

## Request
| Type | Name | Description |
| --- | --- | --- |
| [NotificationEvent](#notificationevent-structure) | oEvent |  |

## Response
This method does not return anything

# Types

## MessageRecipient ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_idRecipient |
| Uint32 | m_uiRecipientType |

## NotificationEvent ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_pidSource |
| Uint32 | m_uiType |
| Uint32 | m_uiParam1 |
| Uint32 | m_uiParam2 |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strParam |
| Uint32 | m_uiParam3 |

## Data ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
This structure does not contain any fields.

## DynamicData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](#data-structure)

| Type | Name |
| --- | --- |
| buffertail | m_bufTail |

## UserMessage ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
> This structure inherits from [Data](#data-structure)

| Type | Name |
| --- | --- |
| Uint32 | m_uiID |
| Uint32 | m_idRecipient |
| Uint32 | m_uiRecipientType |
| Uint32 | m_uiParentID |
| Uint32 | m_pidSender |
| [DateTime](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#datetime) | m_receptiontime |
| Uint32 | m_uiLifeTime |
| Uint32 | m_uiFlags |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strSubject |
| [String](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#string) | m_strSender |

## ResultRange ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_uiOffset |
| Uint32 | m_uiSize |

## Property ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_ID |
| Sint32 | m_value |

## PropertyVariant ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
| Type | Name |
| --- | --- |
| Uint32 | m_ID |
| [Variant](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#variant) | m_value |