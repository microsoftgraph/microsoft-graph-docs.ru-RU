---
title: тип ресурса свойства
description: Определение свойства схемы для Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5581d988cc47d5803e2a753182289458cbeaa747
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665882"
---
# <a name="property-resource-type"></a>тип ресурса свойства

Пространство имен: microsoft.graph.externalConnectors



Определение [свойства схемы](externalconnectors-schema.md) для Поиск (Майкрософт) [подключения.](externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|псевдонимы|Коллекция String|Набор псевдонимов или дружественных имен для свойства. Максимум 32 символа. Каждая строка не должна содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` Необязательно.|
|isQueryable|Логический|Указывает, запрашивается ли свойство. Запрашиваемые свойства можно использовать в запросах На языке запросов ключевых слов [(KQL).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference) Необязательно.|
|isRefinable|Логический|Указывает, является ли свойство уточненным.  Уточненные свойства можно использовать для фильтрации результатов поиска в [API](search-api-overview.md) поиска и добавления управления Поиск (Майкрософт) пользователей. Необязательно.|
|isRetrievable|Логический|Указывает, является ли свойство искомым. Возвращаемые свойства возвращаются в наборе результатов, когда элементы возвращаются API поиска. Свойства, которые можно получить, также доступны для добавления в шаблон отображения, используемый для отрисовки результатов поиска. Необязательно.|
|isSearchable|Логический|Указывает, можно ли найти свойство. Только свойства типа `String` или `StringCollection` можно искать. Невыявимые свойства не добавляются в индекс поиска. Необязательно.|
|метки|коллекция microsoft.graph.externalConnectors.label|Указывает один или несколько известных тегов, добавленных к свойству. Метки помогают Поиск (Майкрософт) понять семантику данных в подключении. Добавление соответствующих меток приведет к усилению поиска (например, повышению релевантности). Возможные значения: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName`, `fileExtension`, `unknownFutureValue`. Необязательно.|
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

