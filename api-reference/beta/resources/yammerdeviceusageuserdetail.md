---
title: Тип ресурса Яммердевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 982ebfc0de39bd956a4223e7bb0665ac73c42402
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519003"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Тип ресурса Яммердевицеусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| репортрефрешдате | Дата    |
| userPrincipalName | String  |
| displayName       | Строка  |
| userState         | String  |
| статечанжедате   | Дата    |
| ластактивитидате  | Дата    |
| уседвеб           | Boolean |
| уседвиндовсфоне  | Boolean |
| уседандроидфоне  | Boolean |
| уседифоне        | Boolean |
| уседипад          | Boolean |
| уседосерс        | Boolean |
| репортпериод      | String  |

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
