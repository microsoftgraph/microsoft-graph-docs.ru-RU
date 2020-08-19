---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 50f37fdfd3441c256241b76ebcc6b144eb1486d7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811055"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| репортрефрешдате | Дата    |
| userPrincipalName | String  |
| ластактивитидате  | Дата    |
| уседвиндовс       | Логический |
| уседвиндовсфоне  | Логический |
| уседандроидфоне  | Логический |
| уседифоне        | Логический |
| уседипад          | Логический |
| репортпериод      | String  |

## <a name="json-representation"></a>Представление в формате JSON

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
