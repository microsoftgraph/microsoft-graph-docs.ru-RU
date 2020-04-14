---
title: Тип ресурса Емаилаппусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8d25f8ce307fb5572515ce12c347fdc2a7dbb726
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440550"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса Емаилаппусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| isDeleted         | Логическое           |
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
