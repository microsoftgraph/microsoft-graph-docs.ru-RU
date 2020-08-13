---
title: Тип ресурса Теамсдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5c3815b2418f414aa552f211bbeed5f643eb0d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519864"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Тип ресурса Теамсдевицеусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| репортрефрешдате | Дата    |
| userPrincipalName | String  |
| ластактивитидате  | Дата    |
| isDeleted         | Логическое |
| делетеддате       | Дата    |
| уседвеб           | Логическое |
| уседвиндовсфоне  | Логическое |
| уседиос           | Логическое |
| уседмак           | Логическое |
| уседандроидфоне  | Логическое |
| уседвиндовс       | Логическое |
| репортпериод      | Строка  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
