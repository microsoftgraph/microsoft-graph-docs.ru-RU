---
title: тип ресурса skypeForBusinessDeviceUsageUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: e243a885f5687042f54f7dd77afe1642f398c99c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063568"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>тип ресурса skypeForBusinessDeviceUsageUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| reportRefreshDate | Дата    |
| userPrincipalName | String  |
| lastActivityDate  | Дата    |
| usedWindows       | Boolean |
| usedWindowsPhone  | Логический |
| usedAndroidPhone  | Boolean |
| usediPhone        | Логический |
| usediPad          | Boolean |
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


