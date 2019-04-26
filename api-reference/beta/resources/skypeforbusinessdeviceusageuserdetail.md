---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555936"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажеусердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| Репортрефрешдате | Дата    |
| userPrincipalName | String  |
| Ластактивитидате  | Дата    |
| Уседвиндовс       | Логический |
| Уседвиндовсфоне  | Логический |
| Уседандроидфоне  | Логический |
| Уседифоне        | Логический |
| Уседипад          | Логический |
| Репортпериод      | String  |

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
