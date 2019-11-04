---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: eed73f61b281463848c8520ebdcdbc75ac26d29d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939336"
---
# <a name="itememail-resource-type"></a>Тип ресурса Итемемаил

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения об адресах электронной почты, связанных с пользователем.

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип               | Описание                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [Получение](../api/itememail-get.md) | [итемемаил](itememail.md) | Чтение свойств и связей объекта **итемемаил** . |
| [Update](../api/itememail-update.md)     | [итемемаил](itememail.md) | Обновление объекта **итемемаил** .                               |
| [Delete](../api/itememail-delete.md)     | Нет.                      | Удаление объекта **итемемаил** .                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|address       |String       | Сам адрес электронной почты.                                                 |
|displayName   |Строка       | Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.  |
|type          |строка       | Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.      |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": ""
}-->

```json
{
  "address": "String",
  "displayName": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemEmail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
