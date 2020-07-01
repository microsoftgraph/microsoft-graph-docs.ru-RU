---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9862170dfcca0960ebd319089da70cca93782875
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990272"
---
# <a name="property-resource-type"></a>Тип ресурса свойства

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание                                        |
|:--------------|:------------------|:---------------------------------------------------|
| псевдоним       | Коллекция String | Набор псевдонимов или понятные имена для свойства. Максимальное число символов 32. Каждая строка не должна содержать управляющие символы, пробелы или любые из следующих элементов: `:` ,, `;` `,` ,, `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, Необязательный параметр.  |
| Queryable   | Boolean           | Указывает, является ли свойство подзапросом. Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Необязательный параметр.  |
| возможность уточнения   | Boolean           | Указывает, является ли свойство уточнением.  Свойства уточнения можно использовать для фильтрации результатов поиска в [API поиска](search-api-overview.md) и добавления уточнения в пользовательский интерфейс поиска Майкрософт. Необязательный параметр.  |
| возможность извлечения | Boolean           | Указывает, может ли свойство быть извлечено. Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска. Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска. Необязательный параметр. |
| с возможностью поиска  | Boolean           | Указывает, доступно ли свойство для поиска. Только свойства типа `String` или `StringCollection` могут быть доступны для поиска. Свойства, не включаемые в поиск, не добавляются в индекс поиска. Необязательный параметр. |
| Метка        | Коллекция String | Указывает один или несколько хорошо известных тегов, добавленных к свойству. Метки помогают Microsoft Search распознавать семантику данных в подключении. Добавление соответствующих меток приведет к расширению возможностей поиска (например, лучшей релевантности). Поддерживаемые Метки:,,,,,, `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` и `fileExtension` . Необязательный параметр. |
| name          | String            | Имя свойства. Максимальное число символов 32. Не должно содержать управляющие символы, пробелы или любые из следующих элементов: `:` ,, `;` `,` ,, `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` ,,, `^` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, Обязательное.                |
| type          | String            | Тип данных указанного свойства. Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`. Обязательный элемент. |

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
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "String" ],
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
