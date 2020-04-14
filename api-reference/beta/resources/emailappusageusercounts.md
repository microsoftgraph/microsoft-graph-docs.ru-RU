---
title: Тип ресурса Емаилаппусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a9878e2f98ca1beff51e6bd9ea803e8cbebeb390
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440557"
---
# <a name="emailappusageusercounts-resource-type"></a>Тип ресурса Емаилаппусажеусеркаунтс

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
| reportDate        | Дата   |
| репортпериод      | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
