---
title: Тип ресурса диагностики
description: Сведения об ошибке или предупреждение для выполнения операции OneNote.
localization_priority: Normal
ms.openlocfilehash: 28cdd1c07bab0494a69cfb7ce6a5284238e1ff19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845992"
---
# <a name="diagnostic-resource-type"></a>Тип ресурса диагностики

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сведения об ошибке или предупреждение для выполнения операции OneNote.

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
|message|String|Сообщение, описывающее условие, инициирующую сообщение об ошибке или предупреждение.|
|url|String|Ссылка на документацию для этой проблемы.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
