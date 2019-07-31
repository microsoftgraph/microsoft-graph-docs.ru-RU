---
title: Тип ресурса Нотебуклинкс
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 866176f1c831c70b7a057d1a53ad6b5fa7e5cda4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966659"
---
# <a name="notebooklinks-resource-type"></a>Тип ресурса Нотебуклинкс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылки для открытия записной книжки OneNote.

## <a name="json-representation"></a>Представление JSON

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
|oneNoteWebUrl|[externalLink](externallink.md)|Открывает записную книжку в OneNote в Интернете.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
