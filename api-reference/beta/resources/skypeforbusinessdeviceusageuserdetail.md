---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 582c3483d4292f634385461508bf579834dfd12e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520410"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| репортрефрешдате | Дата    |
| userPrincipalName | String  |
| ластактивитидате  | Дата    |
| уседвиндовс       | Boolean |
| уседвиндовсфоне  | Boolean |
| уседандроидфоне  | Boolean |
| уседифоне        | Boolean |
| уседипад          | Boolean |
| репортпериод      | String  |

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
