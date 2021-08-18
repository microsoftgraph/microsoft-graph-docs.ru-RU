---
title: тип ресурса emailAppUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dce83b17f029bec2bf8977d0e863dcdb5c7fc4e1a9c5dea731b654d5ce6ab9f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54210073"
---
# <a name="emailappusageuserdetail-resource-type"></a>тип ресурса emailAppUsageUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| reportRefreshDate | Дата              |
| userPrincipalName | String            |
| displayName       | Строка            |
| isDeleted         | Логический           |
| deletedDate       | Дата              |
| lastActivityDate  | Дата              |
| mailForMac        | Коллекция String |
| outlookForMac     | Коллекция String |
| outlookForWindows | Коллекция String |
| outlookForMobile  | Коллекция String |
| otherForMobile    | Коллекция String |
| outlookForWeb     | Коллекция String |
| pop3App           | Коллекция String |
| imap4App          | Коллекция String |
| smtpApp           | Коллекция String |
| reportPeriod      | Строка            |

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


