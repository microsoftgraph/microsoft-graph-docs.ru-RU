---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aaf58bd7e20caeb418946814daa7ca8f7bb9bfa3
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229418"
---
# <a name="itememail-resource-type"></a>Тип ресурса Итемемаил

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения об адресах электронной почты, связанных с пользователем.

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип               | Описание                                                      |
|:-----------------------------------------|:--------------------------|:-----------------------------------------------------------------|
| [получение](../api/itememail-get.md);           | [итемемаил](itememail.md) | Чтение свойств и связей объекта **итемемаил** .    |
| [Обновление](../api/itememail-update.md)     | [итемемаил](itememail.md) | Обновление объекта **итемемаил** .                                  |
| [Удаление](../api/itememail-delete.md)     | Нет                      | Удаление объекта **итемемаил** .                                  |

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
