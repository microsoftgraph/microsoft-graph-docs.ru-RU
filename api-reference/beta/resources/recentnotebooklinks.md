---
title: Тип ресурса recentNotebookLinks
description: Ссылки на открытие записной книжке OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
ms.openlocfilehash: de13f25148425a1816a60f6cf5b9f4a09f61c7dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078396"
---
# <a name="recentnotebooklinks-resource-type"></a>Тип ресурса recentNotebookLinks

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ссылки на открытие записной книжке OneNote. Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает записную книжку в клиент OneNote, если она установлена.|
|oneNoteWebUrl|[externalLink](externallink.md)|Открывает записную книжку в OneNote Online.|

## <a name="json-representation"></a>Описание в формате JSON

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
