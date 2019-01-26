---
title: Тип ресурса yammerDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574154"
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
| usedWeb           | Boolean |
| usedWindowsPhone  | Boolean |
| usedAndroidPhone  | Boolean |
| usediPhone        | Boolean |
| usediPad          | Boolean |
| usedOthers        | Boolean |
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
