---
title: Тип ресурса educationSynchronizationLicenseAssignment
description: Представляет информацию о лицензии для назначения учетных записей пользователей. Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c60b868ab8d973f6249d7e9ea2b30415d4b8a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409680"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>Тип ресурса educationSynchronizationLicenseAssignment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет информацию о лицензии для назначения учетных записей пользователей. Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **appliesTo** | string | Тип роли пользователя для назначения лицензий. Возможные значения: `student`, `teacher`.         |
| **skuIds** | набор строк |  Представляет идентификаторы SKU лицензий для назначения.        |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
