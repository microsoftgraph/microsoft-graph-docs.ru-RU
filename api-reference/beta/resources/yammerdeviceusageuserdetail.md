---
title: Тип ресурса Яммердевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9d12b329767081767b58f4fd36e9eac5edffe406
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979174"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Тип ресурса Яммердевицеусажеусердетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| репортрефрешдате | Дата    |
| userPrincipalName | String  |
| displayName       | String  |
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


