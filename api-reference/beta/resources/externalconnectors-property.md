---
title: тип ресурса свойства
description: Определение свойства схемы для Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8e959839893a106e26f3752c38365b1040743511
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454271"
---
# <a name="property-resource-type"></a>тип ресурса свойства

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определение [свойства схемы](externalconnectors-schema.md) для Поиск (Майкрософт) [подключения.](externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание                                        |
|:--------------|:------------------|:---------------------------------------------------|
| псевдонимы       | Коллекция строк | Набор псевдонимов или дружественных имен для свойства. Максимум 32 символа. Разрешены только буквы. Например, каждая строка не может содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `` ` `` `^` Необязательно.  |
| isQueryable   | boolean           | Указывает, запрашивается ли свойство. Запрашиваемые свойства можно использовать в запросах На языке запросов ключевых слов [(KQL).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference) Необязательно.  |
| isRefinable   | boolean           | Указывает, является ли свойство уточненным.  Уточненные свойства можно использовать для фильтрации результатов поиска в [API](search-api-overview.md) поиска и добавления управления Поиск (Майкрософт) пользователей. Необязательно.  |
| isRetrievable | boolean           | Указывает, является ли свойство искомым. Возвращаемые свойства возвращаются в наборе результатов, когда элементы возвращаются API поиска. Свойства, которые можно получить, также доступны для добавления в шаблон отображения, используемый для отрисовки результатов поиска. Необязательный параметр. |
| isSearchable  | boolean           | Указывает, можно ли найти свойство. Только свойства типа `string` или `stringCollection` можно искать. Невыявимые свойства не добавляются в индекс поиска. Необязательно. |
| метки        | коллекция microsoft.graph.externalConnectors.label | Указывает один или несколько известных тегов, добавленных к свойству. Метки помогают Поиск (Майкрософт) понять семантику данных в подключении. Добавление соответствующих меток приведет к усилению поиска (например, повышению релевантности). Необязательный параметр.<br><br>Возможные значения: `title` , , , , , , , , `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `unknownFutureValue` `iconUrl` `containerName` `containerUrl` . Обратите внимание, что для получения следующих значений в этом изменяемом переумыве: `Prefer: include-unknown-enum-members` , , [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `iconUrl` `containerName` `containerUrl` .|
| name          | String            | Имя свойства. Максимум 32 символа. Разрешены только буквы. Например, каждая строка не может содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `` ` `` `^`  Обязательное.                |
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
