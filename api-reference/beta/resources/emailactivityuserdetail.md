---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 76ec180ceb239f79c420f26b48521e9bc7e81787
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979485"
---
# <a name="emailactivityuserdetail-resource-type"></a>Тип ресурса Емаилактивитюсердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Boolean           |
| делетеддате       | Дата              |
| ластактивитидате  | Дата              |
| сендкаунт         | Int64             |
| рецеивекаунт      | Int64             |
| реадкаунт         | Int64             |
| ассигнедпродуктс  | Коллекция String |
| репортпериод      | String            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```


