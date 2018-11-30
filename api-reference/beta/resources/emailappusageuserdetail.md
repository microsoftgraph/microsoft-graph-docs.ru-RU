---
title: Тип ресурса emailAppUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 951d53f7491ff7f2b7721b14ed354d770cfd1730
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075424"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса emailAppUsageUserDetail

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| reportRefreshDate | Date              |
| userPrincipalName | String            |
| displayName       | String            |
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
