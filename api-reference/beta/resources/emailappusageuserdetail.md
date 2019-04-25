---
title: Тип ресурса Емаилаппусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542841"
---
# <a name="emailappusageuserdetail-resource-type"></a>Тип ресурса Емаилаппусажеусердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип              |
| :---------------- | :---------------- |
| Репортрефрешдате | Дата              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Логический           |
| Делетеддате       | Дата              |
| Ластактивитидате  | Дата              |
| Маилформак        | Коллекция строк |
| Аутлукформак     | Коллекция строк |
| Аутлукфорвиндовс | Коллекция строк |
| Аутлукформобиле  | Коллекция строк |
| Осерформобиле    | Коллекция строк |
| Аутлукфорвеб     | Коллекция строк |
| pop3App           | Коллекция строк |
| imap4App          | Коллекция строк |
| Смтпапп           | Коллекция строк |
| Репортпериод      | String            |

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
