---
title: тип ресурса свойства
description: Определение свойства схемы для Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d15091c9a4f637019cf85cc55011feec86ce44f
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665767"
---
# <a name="property-resource-type"></a>тип ресурса свойства

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определение [свойства схемы](externalconnectors-schema.md) для Поиск (Майкрософт) [подключения.](externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание                                        |
|:--------------|:------------------|:---------------------------------------------------|
| псевдонимы       | Коллекция String | Набор псевдонимов или дружественных имен для свойства. Максимум 32 символа. Каждая строка не должна содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` Необязательно.  |
| isQueryable   | логический           | Указывает, запрашивается ли свойство. Запрашиваемые свойства можно использовать в запросах На языке запросов ключевых слов [(KQL).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference) Необязательно.  |
| isRefinable   | логический           | Указывает, является ли свойство уточненным.  Уточненные свойства можно использовать для фильтрации результатов поиска в [API](search-api-overview.md) поиска и добавления управления Поиск (Майкрософт) пользователей. Необязательно.  |
| isRetrievable | логический           | Указывает, является ли свойство искомым. Возвращаемые свойства возвращаются в наборе результатов, когда элементы возвращаются API поиска. Свойства, которые можно получить, также доступны для добавления в шаблон отображения, используемый для отрисовки результатов поиска. Необязательно. |
| isSearchable  | логический           | Указывает, можно ли найти свойство. Только свойства типа `string` или `stringCollection` можно искать. Невыявимые свойства не добавляются в индекс поиска. Необязательно. |
| метки        | коллекция microsoft.graph.externalConnectors.label | Указывает один или несколько известных тегов, добавленных к свойству. Метки помогают Поиск (Майкрософт) понять семантику данных в подключении. Добавление соответствующих меток приведет к усилению поиска (например, повышению релевантности). Необязательно.<br><br>Возможные значения: `title` , , , , , , , , `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `unknownFutureValue` `iconUrl` `containerName` `containerUrl` . Обратите внимание, что для получения следующих значений в этом изменяемом переумыве: `Prefer: include-unknown-enum-members` , , [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `iconUrl` `containerName` `containerUrl` .|
| name          | String            | Имя свойства. Максимум 32 символа. Не должен содержать символы управления, whitespace или любой из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` Обязательное.                |
| type          | microsoft.graph.externalConnectors.propertyType         | Тип данных указанного свойства. Возможные значения: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`. Обязательный элемент. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "string" ],
  "name": "string",
  "type": "string"
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
