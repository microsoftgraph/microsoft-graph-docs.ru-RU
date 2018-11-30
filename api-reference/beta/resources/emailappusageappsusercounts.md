---
title: Тип ресурса emailAppUsageAppsUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: e588a671129c6aa131bce781e3a6db0d44128f6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077676"
---
# <a name="emailappusageappsusercounts-resource-type"></a>Тип ресурса emailAppUsageAppsUserCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| reportRefreshDate | Date   |
| mailForMac        | Int64  |
| outlookForMac     | Int64  |
| outlookForWindows | Int64  |
| outlookForMobile  | Int64  |
| otherForMobile    | Int64  |
| outlookForWeb     | Int64  |
| pop3App           | Int64  |
| imap4App          | Int64  |
| smtpApp           | Int64  |
| reportPeriod      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportPeriod": "String"
}
```
