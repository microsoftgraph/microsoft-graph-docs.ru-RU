---
title: Тип ресурса Теамсдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007629"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Тип ресурса Теамсдевицеусажеусердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| Репортрефрешдате | Дата    |
| userPrincipalName | String  |
| Ластактивитидате  | Дата    |
| isDeleted         | Boolean |
| Делетеддате       | Дата    |
| Уседвеб           | Boolean |
| Уседвиндовсфоне  | Boolean |
| Уседиос           | Boolean |
| Уседмак           | Boolean |
| Уседандроидфоне  | Boolean |
| Уседвиндовс       | Boolean |
| Репортпериод      | String  |

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
