---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 7a906d0ece395aec191702bcd1b27d2cbea01af2
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236680"
---
# <a name="recentnotebooklinks-resource-type"></a>Тип ресурса recentNotebookLinks

Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает записную книжку в собственном клиенте OneNote, если он установлен.|
|oneNoteWebUrl|[externalLink](externallink.md)|Открывает записную книжку в OneNote в Интернете.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
