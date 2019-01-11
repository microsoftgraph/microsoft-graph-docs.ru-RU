---
title: Тип ресурса emailAppUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 9f1748d6ae3b313fd9f3a87cc211858b5b876b9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858949"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса emailAppUsageUserDetail

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| reportRefreshDate | Date              |
| userPrincipalName | Строка            |
| displayName       | Строка            |
| isDeleted         | Логический           |
| deletedDate       | Date              |
| lastActivityDate  | Date              |
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
