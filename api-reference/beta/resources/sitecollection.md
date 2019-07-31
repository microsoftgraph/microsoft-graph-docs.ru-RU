---
author: JeremyKelley
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0989306be8fa8e456d2718079aec069097cab035
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008294"
---
# <a name="sitecollection-resource"></a>Ресурс SiteCollection

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

| Имя свойства        | Тип     | Описание
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | строка   | Имя узла для семейства веб-сайтов. Только для чтения.
| **Даталокатионкоде** | string   | Код географического региона, в котором располагается это семейство веб-сайтов. Только для чтения.
| **root**             | [root][] | Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint. Только для чтения.

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
