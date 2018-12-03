---
title: Тип ресурса teamsDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082098"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Тип ресурса teamsDeviceUsageUserDetail

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Date    |
| userPrincipalName | String  |
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
