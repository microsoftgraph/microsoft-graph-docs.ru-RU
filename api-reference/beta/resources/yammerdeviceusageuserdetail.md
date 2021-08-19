---
title: тип ресурса yammerDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: e93dde1a1cdd034461a44766df6538da663093ed5d7f4674a3688d0e847aa9f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197774"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>тип ресурса yammerDeviceUsageUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Дата    |
| userPrincipalName | String  |
| displayName       | Строка  |
| userState         | Строка  |
| stateChangeDate   | Дата    |
| lastActivityDate  | Дата    |
| usedWeb           | Логический |
| usedWindowsPhone  | Логический |
| usedAndroidPhone  | Логический |
| usediPhone        | Логический |
| usediPad          | Логический |
| usedOthers        | Логический |
| reportPeriod      | Строка  |

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


