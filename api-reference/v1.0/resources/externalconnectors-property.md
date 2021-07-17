---
title: тип ресурса свойства
description: Определение свойства схемы для Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6159126581d2a95cc45596a29cddff8642c5838f
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467450"
---
# <a name="property-resource-type"></a>тип ресурса свойства

Пространство имен: microsoft.graph.externalConnectors



Определение [свойства схемы](externalconnectors-schema.md) для Поиск (Майкрософт) [подключения.](externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|псевдонимы|Коллекция строк|Набор псевдонимов или дружественных имен для свойства. Максимум 32 символа. Каждая строка не должна содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` Необязательное.|
|isQueryable|Логический|Указывает, запрашивается ли свойство. Запрашиваемые свойства можно использовать в запросах На языке запросов ключевых слов [(KQL).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference) Необязательное.|
|isRefinable|Логический|Указывает, является ли свойство уточненным.  Уточненные свойства можно использовать для фильтрации результатов поиска в [API](search-api-overview.md) поиска и добавления управления Поиск (Майкрософт) пользователей. Необязательное.|
|isRetrievable|Логический|Указывает, является ли свойство искомым. Возвращаемые свойства возвращаются в наборе результатов, когда элементы возвращаются API поиска. Свойства, которые можно получить, также доступны для добавления в шаблон отображения, используемый для отрисовки результатов поиска. Необязательное.|
|isSearchable|Логический|Указывает, можно ли найти свойство. Только свойства типа `String` или `StringCollection` можно искать. Невыявимые свойства не добавляются в индекс поиска. Необязательное.|
|метки|коллекция microsoft.graph.externalConnectors.label|Указывает один или несколько известных тегов, добавленных к свойству. Метки помогают Поиск (Майкрософт) понять семантику данных в подключении. Добавление соответствующих меток приведет к усилению поиска (например, повышению релевантности). Поддерживаемые метки: `title` , , , , , , и `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` . Необязательное.|
|name|String|Имя свойства. Максимум 32 символа. Не должен содержать символы управления, whitespace или любой из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` Обязательное.|
|type|microsoft.graph.externalConnectors.propertyType|Тип данных указанного свойства. Возможные значения: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.property"
}
-->
``` json
{
  "name": "String",
  "type": "String",
  "isSearchable": "Boolean",
  "isRetrievable": "Boolean",
  "isQueryable": "Boolean",
  "isRefinable": "Boolean",
  "aliases": [
    "String"
  ],
  "labels": [
    "String"
  ]
}
```

