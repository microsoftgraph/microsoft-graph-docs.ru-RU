---
title: Тип ресурса Яммердевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 083ace4b10b24e8e5de5d287ddf418d93658c879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006984"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Тип ресурса Яммердевицеусажеусердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| Репортрефрешдате | Дата    |
| userPrincipalName | String  |
| displayName       | Строка  |
| userState         | String  |
| Статечанжедате   | Дата    |
| Ластактивитидате  | Дата    |
| Уседвеб           | Boolean |
| Уседвиндовсфоне  | Boolean |
| Уседандроидфоне  | Boolean |
| Уседифоне        | Boolean |
| Уседипад          | Boolean |
| Уседосерс        | Boolean |
| Репортпериод      | String  |

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
