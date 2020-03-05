---
title: Тип ресурса Персонвебсите
description: Тип ресурса Персонвебсите
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cf4386cf70179715880a1ae07db3dfbb5f07c224
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521899"
---
# <a name="personwebsite-resource-type"></a>Тип ресурса Персонвебсите

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                           | Возвращаемый тип                       | Описание                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [Получение Персонвебсите](../api/personwebsite-get.md) | [персонвебсите](personwebsite.md) | Чтение свойств и связей объекта **персонвебсите** . |
| [Обновление Персонвебсите](../api/personwebsite-update.md)         | [персонвебсите](personwebsite.md) | Обновление объекта **персонвебсите** .                               |
| [Удаление Персонвебсите](../api/personwebsite-delete.md)         | Нет                              | Удаление объекта **персонвебсите** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип              | Описание                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|categories    |Коллекция String  | Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).  |
|description   |String             | Содержит описание веб-сайта.                                              |
|displayName   |Строка             | Содержит понятное имя для веб-сайта.                                           |
|webUrl        |String             | Содержит ссылку на сам веб-сайт.                                              |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personWebsite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
