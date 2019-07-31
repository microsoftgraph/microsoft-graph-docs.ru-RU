---
title: Тип ресурса Теамсусерактивитюсердетаил
description: Ниже приведен пример JSON репресентаион для ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964356"
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
| Ассигнедпродуктс        | Коллекция строк |
| Теамчатмессажекаунт    | Int64             |
| Приватечатмессажекаунт | Int64             |
| Каллкаунт               | Int64             |
| Митингкаунт            | Int64             |
| Хасосерактион          | Boolean           |
| Репортпериод            | String            |

## <a name="json-representation"></a>Представление JSON

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
