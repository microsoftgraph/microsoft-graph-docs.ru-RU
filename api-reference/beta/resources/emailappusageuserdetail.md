---
title: Тип ресурса emailAppUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977656"
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
