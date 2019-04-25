---
title: Тип ресурса Яммердевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551430"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Тип ресурса Яммердевицеусажеусердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| Репортрефрешдате | Дата    |
| userPrincipalName | String  |
| displayName       | String  |
| userState         | String  |
| Статечанжедате   | Дата    |
| Ластактивитидате  | Дата    |
| Уседвеб           | Логический |
| Уседвиндовсфоне  | Логический |
| Уседандроидфоне  | Логический |
| Уседифоне        | Логический |
| Уседипад          | Логический |
| Уседосерс        | Логический |
| Репортпериод      | String  |

## <a name="json-representation"></a>Представление в формате JSON

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
