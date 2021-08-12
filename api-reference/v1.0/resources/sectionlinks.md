---
title: тип ресурса sectionLinks
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c38c7f5418fd0aed2b49db487771795d127ba38dfa2af13c8c7bcbba9d3a2361
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235277"
---
# <a name="sectionlinks-resource-type"></a>тип ресурса sectionLinks

Пространство имен: microsoft.graph

Ссылки для открытия раздела OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
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
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает раздел в OneNote клиенте, если он установлен.|
|oneNoteWebUrl|[externalLink](externallink.md)|Открывает раздел в OneNote в Интернете.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

