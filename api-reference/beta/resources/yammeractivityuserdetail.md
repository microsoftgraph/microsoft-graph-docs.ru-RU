---
title: Тип ресурса Яммерактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 960945d72db1cc347228983b9567968dfcfc52d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963789"
---
# <a name="yammeractivityuserdetail-resource-type"></a>Тип ресурса Яммерактивитюсердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| Репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| userState         | String            |
| Статечанжедате   | Дата              |
| Ластактивитидате  | Дата              |
| Постедкаунт       | Int64             |
| Реадкаунт         | Int64             |
| Ликедкаунт        | Int64             |
| Ассигнедпродуктс  | Коллекция строк |
| Репортпериод      | String            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
