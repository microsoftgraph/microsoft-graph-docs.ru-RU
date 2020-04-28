---
title: Тип ресурса Теамсусерактивитюсердетаил
description: Ниже приведен пример JSON репресентаион для ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 237cfc933cbabd628320131866f7bf24ba0195c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519815"
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
| ассигнедпродуктс        | Коллекция объектов string |
| теамчатмессажекаунт    | Int64             |
| приватечатмессажекаунт | Int64             |
| каллкаунт               | Int64             |
| митингкаунт            | Int64             |
| хасосерактион          | Boolean           |
| репортпериод            | String            |

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
