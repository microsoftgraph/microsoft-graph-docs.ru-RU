---
title: Тип ресурса Яммерактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541187"
---
# <a name="yammeractivityuserdetail-resource-type"></a>Тип ресурса Яммерактивитюсердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| Репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | String            |
| userState         | String            |
| Статечанжедате   | Дата              |
| Ластактивитидате  | Дата              |
| Постедкаунт       | Int64             |
| Реадкаунт         | Int64             |
| Ликедкаунт        | Int64             |
| Ассигнедпродуктс  | Коллекция строк |
| Репортпериод      | String            |

## <a name="json-representation"></a>Представление в формате JSON

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
