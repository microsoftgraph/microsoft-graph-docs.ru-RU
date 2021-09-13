---
title: тип ресурса yammerDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 4a3232f87775f4e08e5296c21282e80ee2f1ee88
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128489"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>тип ресурса yammerDeviceUsageUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Дата    |
| userPrincipalName | String  |
| displayName       | String  |
| userState         | String  |
| stateChangeDate   | Дата    |
| lastActivityDate  | Дата    |
| usedWeb           | Логический |
| usedWindowsPhone  | Логическое |
| usedAndroidPhone  | Логическое |
| usediPhone        | Логический |
| usediPad          | Логический |
| usedOthers        | Логическое |
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


