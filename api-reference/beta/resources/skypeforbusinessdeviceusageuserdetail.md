---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b84cf9c7654354446fb7c6a5005befe3d17a0fa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964916"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>Тип ресурса Скипефорбусинессдевицеусажеусердетаил

## <a name="properties"></a>Свойства

| Свойство          | Тип    |
| :---------------- | :------ |
| Репортрефрешдате | Дата    |
| userPrincipalName | String  |
| Ластактивитидате  | Дата    |
| Уседвиндовс       | Boolean |
| Уседвиндовсфоне  | Boolean |
| Уседандроидфоне  | Boolean |
| Уседифоне        | Boolean |
| Уседипад          | Boolean |
| Репортпериод      | String  |

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
