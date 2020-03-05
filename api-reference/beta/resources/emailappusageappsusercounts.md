---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34ceaf4450a66f07c0678e55db344adc20bb0b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499500"
---
# <a name="emailappusageappsusercounts-resource-type"></a>Тип ресурса Емаилаппусажеаппсусеркаунтс

Пространство имен: Microsoft. Graph

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
