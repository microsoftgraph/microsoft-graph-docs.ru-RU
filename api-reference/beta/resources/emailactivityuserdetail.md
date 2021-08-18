---
title: тип ресурса emailActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a25061ccea7c6971625a96e9ececd60b3f87a9f4817c1aee4c8892385a6c7d55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248980"
---
# <a name="emailactivityuserdetail-resource-type"></a>тип ресурса emailActivityUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| reportRefreshDate | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| isDeleted         | Логический           |
| deletedDate       | Дата              |
| lastActivityDate  | Дата              |
| sendCount         | Int64             |
| receiveCount      | Int64             |
| readCount         | Int64             |
| assignedProducts  | Коллекция String |
| reportPeriod      | Строка            |

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


