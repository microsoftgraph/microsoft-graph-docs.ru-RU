---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0ca694c5d416dcc062984ba03a3521a39a010a87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972182"
---
# <a name="emailappusageappsusercounts-resource-type"></a>Тип ресурса Емаилаппусажеаппсусеркаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| Репортрефрешдате | Дата   |
| Маилформак        | Int64  |
| Аутлукформак     | Int64  |
| Аутлукфорвиндовс | Int64  |
| Аутлукформобиле  | Int64  |
| Осерформобиле    | Int64  |
| Аутлукфорвеб     | Int64  |
| pop3App           | Int64  |
| imap4App          | Int64  |
| Смтпапп           | Int64  |
| Репортпериод      | String |

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
