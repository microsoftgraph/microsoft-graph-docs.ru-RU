---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef2675b8c604115fc5e04a7747dc4c110d567604
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939027"
---
# <a name="personinterest-resource-type"></a>Тип ресурса Персонинтерест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса [персонинтерест](personinterest.md) предоставляет подробные сведения о интересах, которые пользователь связал с самим собой в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [Получение Персонинтерест](../api/personinterest-get.md) | [персонинтерест](personinterest.md) | Чтение свойств и связей объекта Персонинтерест. |
| [Update](../api/personinterest-update.md)          | [персонинтерест](personinterest.md) | Обновление объекта Персонинтерест.                               |
| [Delete](../api/personinterest-delete.md)          | Нет.                                | Удаление объекта Персонинтерест.                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип             | Описание                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|categories    |Коллекция String | Содержит категории, которые пользователь связал с интересом (например: личное, реЦипиес) |
|description   |String            | Содержит описание интереса.                                              |
|displayName   |Строка            | Содержит понятное имя для интереса.                                           |
|webUrl        |String            | Содержит ссылку на веб-страницу или ресурс, представляющие интерес.                         |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

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