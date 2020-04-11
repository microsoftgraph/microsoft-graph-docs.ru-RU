---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d10ea81f3648be1896637ca866d0185c2a674097
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227738"
---
# <a name="personinterest-resource-type"></a>Тип ресурса Персонинтерест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                         | Описание                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
| [Получение Персонинтерест](../api/personinterest-get.md)        | [персонинтерест](personinterest.md) | Чтение свойств и связей объекта **персонинтерест** . |
| [Обновление Персонинтерест](../api/personinterest-update.md)  | [персонинтерест](personinterest.md) | Обновление объекта **персонинтерест** .                                   |
| [Удаление Персонинтерест](../api/personinterest-delete.md)  | Нет                                | Удаление объекта **персонинтерест** .                                   |

## <a name="properties"></a>Свойства

| Свойство     | Тип             | Описание                                                                                    |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------|
|categories    |Коллекция String | Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес). |
|description   |String            | Содержит описание интереса.                                                        |
|displayName   |Строка            | Содержит понятное имя для интереса.                                                     |
|webUrl        |String            | Содержит ссылку на веб-страницу или ресурс, представляющие интерес.                                  |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
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
  "description": "personInterest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
