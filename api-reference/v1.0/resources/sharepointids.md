---
author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
ms.localizationpriority: medium
ms.prod: sharepoint
description: Ресурс SharePointIds — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.
doc_type: resourcePageType
ms.openlocfilehash: 156e2e19d31a15ea2a2790d1286e7515a0214f09
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032253"
---
# <a name="sharepointids-resource-type"></a>Тип ресурса SharePointIds

Пространство имен: microsoft.graph

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
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство         | Тип         | Описание
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.
| listItemId       | string       | Целочисленный идентификатор элемента в списке.
| listItemUniqueId | string       | Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.
| siteId           | string       | Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.
| siteUrl          | string (url) | URL-адрес SharePoint для сайта, содержащего элемент.
| tenantId         | string       | Уникальный идентификатор (guid) для аренды.
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

