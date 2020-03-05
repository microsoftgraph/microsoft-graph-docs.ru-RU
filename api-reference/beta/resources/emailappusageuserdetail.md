---
title: Тип ресурса Емаилаппусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 700ef4b222860d19ef3ba78ae583a50e8cf8d0cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499486"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса Емаилаппусажеусердетаил

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| isDeleted         | Логический           |
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
| репортпериод      | String            |

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
