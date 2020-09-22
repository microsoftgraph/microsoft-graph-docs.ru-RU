---
title: Тип ресурса Теамсусерактивитюсердетаил
description: Ниже приведен пример JSON репресентаион для ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73208044be5d3612303774f92dfced2302939de8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046358"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Тип ресурса Теамсусерактивитюсердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                | Тип              |
| :---------------------- | :---------------- |
| репортрефрешдате       | Дата              |
| userPrincipalName       | String            |
| ластактивитидате        | Дата              |
| isDeleted               | Boolean           |
| делетеддате             | Дата              |
| ассигнедпродуктс        | Коллекция String |
| теамчатмессажекаунт    | Int64             |
| приватечатмессажекаунт | Int64             |
| каллкаунт               | Int64             |
| митингкаунт            | Int64             |
| хасосерактион          | Boolean           |
| репортпериод            | Строка            |

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


