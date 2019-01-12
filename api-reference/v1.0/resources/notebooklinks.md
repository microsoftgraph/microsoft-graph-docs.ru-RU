---
title: Тип ресурса notebookLinks
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d3def81fb9bb3b7f657be3ed04230a65235db5f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984257"
---
# <a name="notebooklinks-resource-type"></a>Тип ресурса notebookLinks

Ссылки для открытия записной книжки OneNote.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
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
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает записную книжку в собственном клиенте OneNote, если он установлен.|
|oneNoteWebUrl|[externalLink](externallink.md)|Открывает записную книжку в OneNote Online.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
