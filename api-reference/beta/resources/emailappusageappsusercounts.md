---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d4dd1bc6a84b1d3e5f1b412986de686c9e6f5312
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979478"
---
# <a name="emailappusageappsusercounts-resource-type"></a>Тип ресурса Емаилаппусажеаппсусеркаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   |
| :---------------- | :----- |
| репортрефрешдате | Дата   |
| маилформак        | Int64  |
| аутлукформак     | Int64  |
| аутлукфорвиндовс | Int64  |
| аутлукформобиле  | Int64  |
| осерформобиле    | Int64  |
| аутлукфорвеб     | Int64  |
| pop3App           | Int64  |
| imap4App          | Int64  |
| смтпапп           | Int64  |
| репортпериод      | String |

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


