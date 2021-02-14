---
author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
doc_type: resourcePageType
ms.openlocfilehash: 1e80ad630fd1ac823ce76c44c3b789b0986d031f
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239438"
---
# <a name="sitecollection-resource"></a>Ресурс SiteCollection

Пространство имен: microsoft.graph

Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.

Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>Свойства

| Имя свойства        | Тип     | Описание
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | строка   | Имя узла для семейства веб-сайтов. Только для чтения.
| **dataLocationCode** | string   | Код географического региона для местоположения этого веб-сайта. Только для чтения.
| **root**             | [root][] | Если указан, означает, что это корневое коллекцию веб-сайтов в SharePoint. Только для чтения.

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->

