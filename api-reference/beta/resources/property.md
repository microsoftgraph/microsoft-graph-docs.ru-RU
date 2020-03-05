---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 48a61c9f26a7f5b90e41fc2cd36334d4061449dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521385"
---
# <a name="property-resource-type"></a>Тип ресурса свойства

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство      | Тип    | Описание                                        |
|:--------------|:--------|:---------------------------------------------------|
| Queryable   | Логический | Указывает, является ли свойство подзапросом. Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Необязательное свойство.  |
| возможность извлечения | Логический | Указывает, может ли свойство быть извлечено. Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска. Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска. Необязательное свойство. |
| с возможностью поиска  | Логический | Указывает, доступно ли свойство для поиска. Только свойства типа `String` или `StringCollection` могут быть доступны для поиска. Свойства, не включаемые в поиск, не добавляются в индекс поиска. Необязательное свойство. |
| name          | String  | Имя свойства. Максимальное число символов 32. Не должно содержать управляющие символы, пробелы или любые из следующих элементов `:`: `;`, `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `<` `>` `|` `` ` `` `^` Обязательное.                |
| type          | String  | Тип данных указанного свойства. Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`. Обязательный элемент. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "name": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
