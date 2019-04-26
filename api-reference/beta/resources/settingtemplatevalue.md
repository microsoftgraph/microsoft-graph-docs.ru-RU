---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
ms.openlocfilehash: 2277f4b7bb66839164a1b09011d20886baf2bd1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343187"
---
# <a name="settingtemplatevalue-resource-type"></a>Тип ресурса Сеттингтемплатевалуе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Значение|string|Значение по умолчанию для параметра. Только для чтения.|
|description|string|Описание параметра. Только для чтения.|
|name|строка|Имя параметра. Только для чтения.|
|type|string|Тип параметра. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
