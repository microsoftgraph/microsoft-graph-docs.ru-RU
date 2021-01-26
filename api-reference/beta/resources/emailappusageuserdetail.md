---
title: Тип ресурса emailAppUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fb6dded6e7c86644191f1d941900050813b84594
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981818"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса emailAppUsageUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| reportRefreshDate | Дата              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Boolean           |
| deletedDate       | Дата              |
| lastActivityDate  | Дата              |
| mailForMac        | Коллекция String |
| outlookForMac     | Коллекция String |
| outlookForWindows | Коллекция String |
| outlookForMobile  | Коллекция String |
| otherForMobile    | Коллекция String |
| outlookForWeb     | Коллекция String |
| pop3App           | Коллекция String |
| imap4App          | Коллекция String |
| smtpApp           | Коллекция String |
| reportPeriod      | String            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "mailForMac": ["String"], 
  "outlookForMac": ["String"], 
  "outlookForWindows": ["String"], 
  "outlookForMobile": ["String"], 
  "otherForMobile": ["String"], 
  "outlookForWeb": ["String"], 
  "pop3App": ["String"], 
  "imap4App": ["String"], 
  "smtpApp": ["String"], 
  "reportPeriod": "String"
}
```


