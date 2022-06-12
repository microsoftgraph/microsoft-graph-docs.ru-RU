---
title: Тип ресурса pageLinks
description: Ссылки для открытия OneNote страницы.
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: 78635d0158cbe1d43833b437edf54db15e10a895
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034728"
---
# <a name="pagelinks-resource-type"></a>Тип ресурса pageLinks

Пространство имен: microsoft.graph

Ссылки для открытия OneNote страницы.

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
|oneNoteClientUrl|[externalLink](externallink.md)|Открывает страницу в OneNote клиенте, если он установлен.|
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

