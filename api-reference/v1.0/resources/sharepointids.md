---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 36636ead90d8b913de4328aea9b6252e82f30c26
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="sharepointids-resource-type"></a>Тип ресурса SharePointIds

Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.

**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство         | Тип         | Описание
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.
| listItemId       | string       | Целочисленный идентификатор элемента в списке.
| listItemUniqueId | строка       | Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.
| siteId           | string       | Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.
| siteUrl          | string (url) | URL-адрес SharePoint для сайта, содержащего элемент.
| webId            | string       | Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
