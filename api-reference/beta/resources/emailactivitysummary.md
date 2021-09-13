---
title: тип ресурса emailActivitySummary
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae2c1d52ab736106f9f76ef07b93b09db4de4d94
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129301"
---
# <a name="emailactivitysummary-resource-type"></a>тип ресурса emailActivitySummary

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Дата   |
| Отправить              | Int64  |
| получение           | Int64  |
| read              | Int64  |
| reportDate        | Дата   |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


