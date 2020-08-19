---
title: Тип ресурса Скипефорбусинессактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 66453b6d8889f4d6bf1be22c41bd534daa94dc72
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811079"
---
# <a name="skypeforbusinessactivityuserdetail-resource-type"></a>Тип ресурса Скипефорбусинессактивитюсердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                                 | Тип              |
| :--------------------------------------- | :---------------- |
| тоталпиртопирсессионкаунт              | Int64             |
| тоталорганизедконференцекаунт            | Int64             |
| тоталпартиЦипатедконференцекаунт         | Int64             |
| пиртопирластактивитидате               | Дата              |
| организедконференцеластактивитидате      | Дата              |
| партиЦипатедконференцеластактивитидате   | Дата              |
| пиртопиримкаунт                        | Int64             |
| пиртопираудиокаунт                     | Int64             |
| пиртопираудиоминутес                   | Int64             |
| пиртопирвидеокаунт                     | Int64             |
| пиртопирвидеоминутес                   | Int64             |
| пиртопираппшарингкаунт                | Int64             |
| пиртопирфилетрансферкаунт              | Int64             |
| организедконференцеимкаунт               | Int64             |
| организедконференцеаудиовидеокаунт       | Int64             |
| организедконференцеаудиовидеоминутес     | Int64             |
| организедконференцеаппшарингкаунт       | Int64             |
| организедконференцевебкаунт              | Int64             |
| organizedConferenceDialInOut3rdPartyCount | Int64             |
| организедконференцеклауддиалинаутмикрософткаунт | Int64             |
| организедконференцеклауддиалинмикрософтминутес | Int64             |
| организедконференцеклауддиалаутмикрософтминутес | Int64             |
| партиЦипатедконференцеимкаунт           | Int64             |
| партиЦипатедконференцеаудиовидеокаунт   | Int64             |
| партиЦипатедконференцеаудиовидеоминутес | Int64             |
| партиЦипатедконференцеаппшарингкаунт   | Int64             |
| партиЦипатедконференцевебкаунт          | Int64             |
| participatedConferenceDialInOut3rdPartyCount | Int64             |
| репортрефрешдате                        | Дата              |
| userPrincipalName                        | String            |
| isDeleted                                | Логический           |
| делетеддате                              | Дата              |
| ластактивитидате                         | Дата              |
| ассигнедпродуктс                         | Коллекция String |
| репортпериод                             | String            |

## <a name="json-representation"></a>Представление в формате JSON

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
