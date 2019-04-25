---
title: Тип ресурса Теамсусерактивитюсердетаил
description: Ниже приведен пример JSON репресентаион для ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582908"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Тип ресурса Теамсусерактивитюсердетаил

## <a name="properties"></a>Свойства

| Свойство                | Тип              |
| :---------------------- | :---------------- |
| Репортрефрешдате       | Дата              |
| userPrincipalName       | String            |
| Ластактивитидате        | Дата              |
| isDeleted               | Boolean           |
| Делетеддате             | Дата              |
| Ассигнедпродуктс        | Коллекция String |
| Теамчатмессажекаунт    | Int64             |
| Приватечатмессажекаунт | Int64             |
| Каллкаунт               | Int64             |
| Митингкаунт            | Int64             |
| Хасосерактион          | Boolean           |
| Репортпериод            | String            |

## <a name="json-representation"></a>Описание в формате JSON

Ниже приведен пример JSON репресентаион для ресурса.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
