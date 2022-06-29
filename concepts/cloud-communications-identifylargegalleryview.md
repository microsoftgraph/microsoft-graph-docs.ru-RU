---
title: Определение участников больших представлений коллекции с помощью API облачных коммуникаций
description: Определите участника большого представления коллекции в списке, чтобы вы могли подписаться на его видеопоток с помощью API облачных коммуникаций в Microsoft Graph.
author: navali-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 55e31cabff32f082ce03d2258fee0bf37fcd3ff4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436206"
---
# <a name="identify-large-gallery-view-participants-in-a-roster"></a>Определение участников представления большой коллекции в списке

API облачных коммуникаций в Microsoft Graph предоставляет конечную точку для добавления представления большой [коллекции в вызов](/graph/api/call-addlargegalleryview) . После успешного добавления представления большой коллекции в вызов можно подписаться на видеопоток участника.

В этой статье описывается, как определить участника большого представления коллекции в списке, чтобы получить соответствующие данные для подписки на видеопоток.

## <a name="roster-example-with-large-gallery-view-participant"></a>Пример списка с большим участником представления коллекции

В следующем примере показан список, который приложение получает после успешного добавления в вызов представления большой коллекции.

```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/5f201300-df95-4800-bd3a-75b0af63dd2b/participants",
      "resourceUrl": "/communications/calls/5f201300-df95-4800-bd3a-75b0af63dd2b/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD",
              }
            },
            "endpointType": "default",
            "endpointId": "40213cfb-0934-4dce-9b3a-57c09adf6967",
            "participantId": "23aeb644-6227-4f4a-b5c9-4d61c1f196d3",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2472",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "23aeb644-6227-4f4a-b5c9-4d61c1f196d3"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD"
              }
            },
            "endpointType": "default",
            "endpointId": "4a767d9b-dca5-4176-8f1b-2a0f98923569",
            "participantId": "63ce9188-e754-4733-9e71-ccc829499a63",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1652",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "1653",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "1655",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "1656",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "63ce9188-e754-4733-9e71-ccc829499a63"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "identityProvider": "AAD",
                "ApplicationType": "LargeGallery-V2"
              }
            },
            "endpointType": "default",
            "endpointId": "ccf24195-bd6d-4cbe-bc46-180a7fd3e9ba",
            "participantId": "a34eae65-7aca-43ab-8332-80ab28629a54",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2886",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "2887",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "metadata": "{\"__platform\":{\"ui\":{\"hidden\":true}},\"audienceView\":{\"id\":\"3c28fd97-6d51-4f2f-8bba-82dcbf408ff6/1\",\"page\":1,\"status\":\"active\",\"type\":\"lg\",\"aspectRatio\":\"widescreen\"}}",
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "a34eae65-7aca-43ab-8332-80ab28629a54"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "identityProvider": "AAD",
                "ApplicationType": "LargeGallery-V2"
              }
            },
            "endpointType": "default",
            "endpointId": "22726e72-fbf4-46c7-a5d7-36c682c3ba86",
            "participantId": "8c4ca6bc-33e1-4da5-b6d6-a2fe61af605d",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2673",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "2674",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "2685",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "metadata": "{\"__platform\":{\"ui\":{\"hidden\":true}}}",
          "isMuted": false,
          "isInLobby": false,
          "meetingRole": "presenter",
          "id": "8c4ca6bc-33e1-4da5-b6d6-a2fe61af605d"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD"
              }
            },
            "endpointType": "default",
            "endpointId": "c2bba3c4-ffff-ffff-eca6-782d381190f4",
            "participantId": "3855ce6a-064e-402c-a1cf-2d78b4e1efbb",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "201",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "202",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "212",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "213",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "metadata": "{\"holographicCapabilities\":3}",
          "isMuted": true,
          "isInLobby": false,
          "meetingRole": "organizer",
          "id": "3855ce6a-064e-402c-a1cf-2d78b4e1efbb"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "(redacted)",
                "displayName": "(redacted)",
                "identityProvider": "AAD"
              }
            },
            "endpointType": "default",
            "endpointId": "b8e00934-5ae7-4e8b-9933-1ed41d70e8c0",
            "participantId": "f65b97d2-efda-471e-a2c5-bfe40146b11f",
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2267",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "label": "main-video",
              "sourceId": "2268",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "2270",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "data",
              "label": "data",
              "sourceId": "2271",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "publishedStates": [],
          "meetingRole": "presenter",
          "id": "f65b97d2-efda-471e-a2c5-bfe40146b11f"
        }
      ]
    }
  ]
}
```

## <a name="identify-large-gallery-view-participants"></a>Определение участников представления "Большая галерея"

Используйте следующие данные из примера списка, чтобы определить участника представления большой коллекции:

- **ApplicationType** участника будет задано как .`LargeGallery-V2`
- Направление **видеопотока** будет установлено в значение `sendReceive`.
- Будут **включены метаданные** , которые будут содержать дополнительные сведения, такие как разбиение по страницам.

### <a name="participant-data-example"></a>Пример данных участника

В следующем примере показаны данные для большого участника представления коллекции в списке.

```json
{
    "@odata.type": "#microsoft.graph.participant",
    "info": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "application": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "(redacted)",
        "identityProvider": "AAD",
        "ApplicationType": "LargeGallery-V2"
        }
    },
    "endpointType": "default",
    "endpointId": "ccf24195-bd6d-4cbe-bc46-180a7fd3e9ba",
    "participantId": "a34eae65-7aca-43ab-8332-80ab28629a54",
    },
    "mediaStreams": [
    {
        "@odata.type": "#microsoft.graph.mediaStream",
        "mediaType": "audio",
        "label": "main-audio",
        "sourceId": "2886",
        "direction": "receiveOnly",
        "serverMuted": false
    },
    {
        "@odata.type": "#microsoft.graph.mediaStream",
        "mediaType": "video",
        "label": "main-video",
        "sourceId": "2887",
        "direction": "sendReceive",
        "serverMuted": false
    }
    ],
    "metadata": "{\"__platform\":{\"ui\":{\"hidden\":true}},\"audienceView\":{\"id\":\"3c28fd97-6d51-4f2f-8bba-82dcbf408ff6/1\",\"page\":1,\"status\":\"active\",\"type\":\"lg\",\"aspectRatio\":\"widescreen\"}}",
    "isMuted": false,
    "isInLobby": false,
    "meetingRole": "presenter",
    "id": "a34eae65-7aca-43ab-8332-80ab28629a54"
}
```

### <a name="definition-for-deserializing-metadata"></a>Определение для десериализации метаданных

Используйте следующее определение для десериализации свойства **метаданных** и извлечения соответствующей информации.

```csharp
    /// <summary>
    /// Metadata for large gallery view
    /// </summary>
    [DataContract]
    public class AudienceView
    {
        /// <summary>
        /// Unique view id
        /// </summary>
        [DataMember(Name = "id")]
        public string Id { get; set; }

        /// <summary>
        /// Page Number
        /// </summary>
        [DataMember(Name = "page")]
        public int Page { get; set; }

        /// <summary>
        /// Signal that page is Active/Inactive
        /// </summary>
        [DataMember(Name = "status")]
        public string Status { get; set; }
    }
```

## <a name="see-also"></a>См. также

- [Общие сведения об API облачных коммуникаций](cloud-communications-concept-overview.md)