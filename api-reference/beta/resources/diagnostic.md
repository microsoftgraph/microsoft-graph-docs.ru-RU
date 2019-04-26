---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждении для операции OneNote.
localization_priority: Normal
ms.openlocfilehash: 63e146cd44e3e2866d9d632fb78cbc222443c9d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340870"
---
# <a name="diagnostic-resource-type"></a>Тип ресурса диагностики

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения об ошибке или предупреждении для операции OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message|String|Сообщение с описанием условия, вызвавшего ошибку или предупреждение.|
|url|String|Ссылка на документацию по этой ошибке.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
