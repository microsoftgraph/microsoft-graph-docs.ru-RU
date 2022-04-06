---
author: JeremyKelley
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
ms.date: 09/10/2017
title: SiteCollection
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1a2d685382eb96d332408a0f03131b5ab0cd6d02
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720845"
---
# <a name="sitecollection-resource"></a>Ресурс SiteCollection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.

Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
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

| Свойство             | Тип     | Описание                                                                         |
| :------------------- | :------- | :---------------------------------------------------------------------------------- |
| **hostname**         | строка   | Имя узла для семейства веб-сайтов. Только для чтения.                                    |
| **dataLocationCode** | строка   | Код географического региона для того, где находится эта коллекция сайтов. Только для чтения.       |
| **root**             | [root][] | При этом указывается, что это корневой набор сайтов в SharePoint. Только для чтения. |

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
