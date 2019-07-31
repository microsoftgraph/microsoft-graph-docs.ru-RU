---
title: Тип ресурса localeInfo
description: Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2d359735d9ac0cc00643b323a056acbb7d44365a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009974"
---
# <a name="localeinfo-resource-type"></a>Тип ресурса localeInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о языковом стандарте, в частности предпочитаемом языке и стране или регионе, вошедшего пользователя.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|языковые стандарты|string|Представления языкового стандарта для пользователя, которое включает предпочитаемый язык и страну или регион. Пример: "en-us". В языковом компоненте используются коды из двух букв, определенные в стандарте [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm), а в компоненте страны — коды из стандарта [ISO 3166-1 alpha-2](https://www.iso.org/iso/country_codes.htm).|
|displayName|string|Имя, представляющее языковой стандарт пользователя на естественном языке, например "Английский (США)".|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
