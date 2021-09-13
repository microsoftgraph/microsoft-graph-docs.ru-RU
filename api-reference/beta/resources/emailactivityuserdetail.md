---
title: тип ресурса emailActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3970874e0f29acaf6f91da4061154d6f610ed32e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136707"
---
# <a name="emailactivityuserdetail-resource-type"></a>тип ресурса emailActivityUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| reportRefreshDate | Дата              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Логическое           |
| deletedDate       | Дата              |
| lastActivityDate  | Дата              |
| sendCount         | Int64             |
| receiveCount      | Int64             |
| readCount         | Int64             |
| assignedProducts  | Коллекция объектов string |
| reportPeriod      | String            |

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


