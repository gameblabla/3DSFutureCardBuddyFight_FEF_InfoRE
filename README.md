# Readme

Network information about Future Card BuddyFight FEF (Future Card Buddyfight Yuujou no Bakunetsu Fight!) released in 2015.

# new-viewer

I added support for it in nex-viewer 

https://github.com/gameblabla/nex-viewer/commit/2521cc11dd89011fe6824f8d01da1498dbc9e8a7

The output log from nex-viewer on 110101_021431 - Buddyfight fight, buddyfight_match_online_match_win_complete_youtu.be 2FdIFeYXXNk can be found in the nex-viewer folder of this repo.

Here's a list of what it found in my dumps :
```
protocolName: 'Authentication'
methodName: 'LoginEx'

protocolName: 'Authentication'
methodName: 'RequestTicket'

protocolName: 'Secure Connection'
methodName: 'Register'

protocolName: 'Matchmake extension'
methodName: 'AutoMatchmakeWithSearchCriteria_Postpone'

protocolName: 'NAT Traversal'
methodName: 'ReportNATProperties'

protocolName: 'Secure Connection'
methodName: 'ReplaceURL'

protocolName: 'Secure Connection'
methodName: 'SendReport'

protocolName: 'Matchmake extension'
methodName: 'OpenParticipation'

protocolName: 'NAT Traversal'
methodName: 'ReportNATProperties'

protocolName: 'Matchmake extension'
methodName: 'OpenParticipation'

protocolName: 'Notification events'
methodName: 'ProcessNotificationEvent'

protocolName: 'NAT Traversal'
methodName: 'InitiateProbe'

protocolName: 'NAT Traversal'
methodName: 'RequestProbeInitiationExt'

protocolName: 'Match making'
methodName: 'UnregisterGathering'
```

# Pcaps network dumps

Network dumps can be found within the pcaps folder.
I also shot a (poorly edited) video with it for one of the dumps (only includes the actual match however).

# nex-documentation-generator

nex-documentation-generator gave me the following output :

[ℹ] Found NEX protocol: HealthProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/HealthProtocol.md

[ℹ] Found NEX protocol: MonitoringProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/MonitoringProtocol.md

[ℹ] Found NEX protocol: NotificationProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/NotificationProtocol.md

[ℹ] Found NEX protocol: RemoteLogDeviceProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/RemoteLogDeviceProtocol.md

[ℹ] Found NEX protocol: TicketGrantingProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/TicketGrantingProtocol.md

[ℹ] Found NEX protocol: SecureConnectionProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/SecureConnectionProtocol.md

[ℹ] Found NEX protocol: NintendoNotificationEventProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/NintendoNotificationEventProtocol.md

[ℹ] Found NEX protocol: AccountManagementProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/AccountManagementProtocol.md

[⚠] Found DDL tree with no protocol declaration. Writing to ./docs/BuddyFight_FEF/ddl-1.json

[⚠] Found DDL tree with no protocol declaration. Writing to ./docs/BuddyFight_FEF/ddl-3.json

[⚠] Found DDL tree with no protocol declaration. Writing to ./docs/BuddyFight_FEF/ddl-5.json

[⚠] Found DDL tree with no protocol declaration. Writing to ./docs/BuddyFight_FEF/ddl-7.json

[ℹ] Found NEX protocol: MatchMakingProtocol
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/MatchMakingProtocol.md

[ℹ] Found NEX protocol: MatchMakingProtocolExt
[✔] Writing protocol documentation to ./docs/BuddyFight_FEF/MatchMakingProtocolExt.md

[⚠] Found DDL tree with no protocol declaration. Writing to ./docs/BuddyFight_FEF/ddl-9.json

[⚠] Found DDL tree with no protocol declaration. Writing to ./docs/BuddyFight_FEF/ddl-11.json

