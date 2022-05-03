---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия OneNote записной книжки. Этот тип ресурса существует как свойство ресурса recentNotebook.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: bb9b7836569ed040a1b2f5c14b7e4a4ed458b983
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176882"
---
# <a name="recentnotebooklinks-resource-type"></a>Тип ресурса recentNotebookLinks

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылки для открытия OneNote записной книжки. Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает записную книжку в OneNote клиенте, если она установлена.|
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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


