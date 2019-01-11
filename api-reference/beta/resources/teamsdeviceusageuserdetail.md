---
title: Тип ресурса teamsDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807107"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Тип ресурса teamsDeviceUsageUserDetail

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Date    |
| userPrincipalName | Строка  |
| lastActivityDate  | Date    |
| isDeleted         | Логический |
| deletedDate       | Date    |
| usedWeb           | Логический |
| usedWindowsPhone  | Логический |
| usediOS           | Логический |
| usedMac           | Логический |
| usedAndroidPhone  | Логический |
| usedWindows       | Логический |
| reportPeriod      | String  |

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
