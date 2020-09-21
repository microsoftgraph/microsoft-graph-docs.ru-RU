---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5aea834ff2943046aff8a390ae110d775fd2f20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989642"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>Тип ресурса Едукатионсинчронизатионлиценсеассигнмент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.

## <a name="properties"></a>Свойства

| Свойство  | Тип              | Описание                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| Тег | String            | Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`, `faculty`. |
| скуидс    | Коллекция String | Представляет идентификаторы SKU назначаемых лицензий.                                      |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "skuIds": ["String"]
}
```


