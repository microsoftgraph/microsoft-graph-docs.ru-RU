---
title: Тип ресурса Скипефорбусинессактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bd17deab26b061f48f762bf8ffeb5f8289b2a51f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008196"
---
# <a name="skypeforbusinessactivityuserdetail-resource-type"></a>Тип ресурса Скипефорбусинессактивитюсердетаил

## <a name="properties"></a>Свойства

| Свойство                                 | Тип              |
| :--------------------------------------- | :---------------- |
| Тоталпиртопирсессионкаунт              | Int64             |
| Тоталорганизедконференцекаунт            | Int64             |
| ТоталпартиЦипатедконференцекаунт         | Int64             |
| Пиртопирластактивитидате               | Дата              |
| Организедконференцеластактивитидате      | Дата              |
| ПартиЦипатедконференцеластактивитидате   | Дата              |
| Пиртопиримкаунт                        | Int64             |
| Пиртопираудиокаунт                     | Int64             |
| Пиртопираудиоминутес                   | Int64             |
| Пиртопирвидеокаунт                     | Int64             |
| Пиртопирвидеоминутес                   | Int64             |
| Пиртопираппшарингкаунт                | Int64             |
| Пиртопирфилетрансферкаунт              | Int64             |
| Организедконференцеимкаунт               | Int64             |
| Организедконференцеаудиовидеокаунт       | Int64             |
| Организедконференцеаудиовидеоминутес     | Int64             |
| Организедконференцеаппшарингкаунт       | Int64             |
| Организедконференцевебкаунт              | Int64             |
| organizedConferenceDialInOut3rdPartyCount | Int64             |
| Организедконференцеклауддиалинаутмикрософткаунт | Int64             |
| Организедконференцеклауддиалинмикрософтминутес | Int64             |
| Организедконференцеклауддиалаутмикрософтминутес | Int64             |
| ПартиЦипатедконференцеимкаунт           | Int64             |
| ПартиЦипатедконференцеаудиовидеокаунт   | Int64             |
| ПартиЦипатедконференцеаудиовидеоминутес | Int64             |
| ПартиЦипатедконференцеаппшарингкаунт   | Int64             |
| ПартиЦипатедконференцевебкаунт          | Int64             |
| participatedConferenceDialInOut3rdPartyCount | Int64             |
| Репортрефрешдате                        | Дата              |
| userPrincipalName                        | String            |
| isDeleted                                | Boolean           |
| Делетеддате                              | Дата              |
| Ластактивитидате                         | Дата              |
| Ассигнедпродуктс                         | Коллекция строк |
| Репортпериод                             | String            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```json
{
  "totalPeerToPeerSessionCount": 1024, 
  "totalOrganizedConferenceCount": 1024, 
  "totalParticipatedConferenceCount": 1024, 
  "peerToPeerLastActivityDate": "Date", 
  "organizedConferenceLastActivityDate": "Date", 
  "participatedConferenceLastActivityDate": "Date", 
  "peerToPeerIMCount": 1024, 
  "peerToPeerAudioCount": 1024, 
  "peerToPeerAudioMinutes": 1024, 
  "peerToPeerVideoCount": 1024, 
  "peerToPeerVideoMinutes": 1024, 
  "peerToPeerAppSharingCount": 1024, 
  "peerToPeerFileTransferCount": 1024, 
  "organizedConferenceIMCount": 1024, 
  "organizedConferenceAudioVideoCount": 1024, 
  "organizedConferenceAudioVideoMinutes": 1024, 
  "organizedConferenceAppSharingCount": 1024, 
  "organizedConferenceWebCount": 1024, 
  "organizedConferenceDialInOut3rdPartyCount": 1024, 
  "organizedConferenceCloudDialInOutMicrosoftCount": 1024, 
  "organizedConferenceCloudDialInMicrosoftMinutes": 1024, 
  "organizedConferenceCloudDialOutMicrosoftMinutes": 1024, 
  "participatedConferenceIMCount": 1024, 
  "participatedConferenceAudioVideoCount": 1024, 
  "participatedConferenceAudioVideoMinutes": 1024, 
  "participatedConferenceAppSharingCount": 1024, 
  "participatedConferenceWebCount": 1024, 
  "participatedConferenceDialInOut3rdPartyCount": 1024, 
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
