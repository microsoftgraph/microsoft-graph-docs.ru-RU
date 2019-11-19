---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 465ad0824bf46949476304905bf0fea5c3ff6271
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703772"
---
# <a name="property-resource-type"></a>Тип ресурса свойства

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство      | Тип    | Описание                                        |
|:--------------|:--------|:---------------------------------------------------|
| Queryable   | Логическое | Указывает, является ли свойство подзапросом. Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Необязательный параметр.  |
| возможность извлечения | Логическое | Указывает, может ли свойство быть извлечено. Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска. Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска. Необязательный параметр. |
| с возможностью поиска  | Логическое | Указывает, доступно ли свойство для поиска. Только свойства типа `String` или `Collection(String)` могут быть доступны для поиска. Свойства, не включаемые в поиск, не добавляются в индекс поиска. Необязательный параметр. |
| name          | String  | Имя свойства. Максимальное число символов 32. Не должно содержать управляющие символы, пробелы или любые из следующих элементов `:`: `;`, `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `<` `>` `|` `` ` `` `^` Обязательное.                |
| type          | String  | Тип данных указанного свойства. Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`. Обязательный элемент. |

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
