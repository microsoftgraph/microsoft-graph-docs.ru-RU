---
author: JeremyKelley
description: Ресурс SharePointIds — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e22c653bf2dd88fe75fdb43dd8e9601c2a9d6d4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520690"
---
# <a name="sharepointids-resource-type"></a>Тип ресурса SharePointIds

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| tenantId         | string       | Уникальный идентификатор (GUID) для клиента.
| webId            | string       | Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": []
}
-->
