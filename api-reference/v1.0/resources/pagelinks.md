---
title: Тип ресурса Пажелинкс
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: 54121a6232ae02d12571f925909be5b92a2bb0cd
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236610"
---
# <a name="pagelinks-resource-type"></a>Тип ресурса Пажелинкс

Ссылки для открытия страницы OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает страницу в собственном клиенте OneNote, если она установлена.|
|oneNoteWebUrl|[externalLink](externallink.md)|Открывает страницу в OneNote в Интернете.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
