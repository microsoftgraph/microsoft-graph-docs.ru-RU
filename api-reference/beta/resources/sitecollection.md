---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7fb11fc9dc2f55b853ec512255ffa06f8a53cef6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933675"
---
# <a name="sitecollection-resource"></a>Ресурс SiteCollection

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.

Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.

## <a name="json-representation"></a>Представление в формате JSON

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
| **dataLocationCode** | строка   | Код географического региона для размещения семейства веб-сайтов. Только для чтения.
| **root**             | [root][] | Если этот параметр указан, указывает, что это корневого семейства сайтов в SharePoint. Только для чтения.

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
