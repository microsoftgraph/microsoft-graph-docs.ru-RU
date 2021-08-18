---
title: тип ресурса skypeForBusinessDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: d3a37dd171cbd6d3df357bcd978fecad2b3b4c04f31e2238668ab6842c9370cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241305"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>тип ресурса skypeForBusinessDeviceUsageUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Дата    |
| userPrincipalName | String  |
| lastActivityDate  | Дата    |
| usedWindows       | Логический |
| usedWindowsPhone  | Логический |
| usedAndroidPhone  | Логический |
| usediPhone        | Логический |
| usediPad          | Логический |
| reportPeriod      | String  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "lastActivityDate": "Date",
  "usedWindows": true,
  "usedWindowsPhone": true,
  "usedAndroidPhone": true,
  "usediPhone": true,
  "usediPad": true,
  "reportPeriod": "String"
}
```


