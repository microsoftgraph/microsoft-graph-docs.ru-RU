---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 54efe4d3a24a0409e8daa2ebde6d4aff4b729118
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440571"
---
# <a name="emailactivityuserdetail-resource-type"></a>Тип ресурса Емаилактивитюсердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| isDeleted         | Логическое           |
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
