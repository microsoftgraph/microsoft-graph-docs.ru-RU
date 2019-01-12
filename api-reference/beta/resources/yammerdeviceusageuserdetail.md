---
title: Тип ресурса yammerDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2b74222c1a636fac271268e228c8140e7d1cf33f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912010"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Тип ресурса yammerDeviceUsageUserDetail

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Date    |
| userPrincipalName | Строка  |
| displayName       | Строка  |
| userState         | Строка  |
| stateChangeDate   | Date    |
| lastActivityDate  | Date    |
| usedWeb           | Логический |
| usedWindowsPhone  | Логический |
| usedAndroidPhone  | Логический |
| usediPhone        | Логический |
| usediPad          | Логический |
| usedOthers        | Логический |
| reportPeriod      | String  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
