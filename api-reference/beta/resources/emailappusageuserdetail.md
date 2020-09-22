---
title: Тип ресурса Емаилаппусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8365e856ee1b34b15b1aea3369b6cc22f99991e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081680"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса Емаилаппусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| isDeleted         | Boolean           |
| делетеддате       | Дата              |
| ластактивитидате  | Дата              |
| маилформак        | Коллекция String |
| аутлукформак     | Коллекция String |
| аутлукфорвиндовс | Коллекция String |
| аутлукформобиле  | Коллекция String |
| осерформобиле    | Коллекция String |
| аутлукфорвеб     | Коллекция String |
| pop3App           | Коллекция String |
| imap4App          | Коллекция String |
| смтпапп           | Коллекция String |
| репортпериод      | Строка            |

## <a name="json-representation"></a>Представление в формате JSON

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


