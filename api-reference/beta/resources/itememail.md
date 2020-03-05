---
title: Тип ресурса Итемемаил
description: Тип ресурса Итемемаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a18d72fb44f373b6cee1047cc2eed5f0c18a1d0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523081"
---
# <a name="itememail-resource-type"></a>Тип ресурса Итемемаил

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения об адресах электронной почты, связанных с пользователем.

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип               | Описание                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [получение](../api/itememail-get.md); | [итемемаил](itememail.md) | Чтение свойств и связей объекта **итемемаил** . |
| [обновление](../api/itememail-update.md).     | [итемемаил](itememail.md) | Обновление объекта **итемемаил** .                               |
| [удаление](../api/itememail-delete.md);     | Нет                      | Удаление объекта **итемемаил** .                               |

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
