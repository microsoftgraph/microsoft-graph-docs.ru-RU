---
title: Тип ресурса educationLinkResource
description: Подкласс educationResource. Этот ресурс является ссылкой и не имеют дополнительные данные, связанные с ним.
author: mmast-msft
ms.openlocfilehash: 02a55eeea25ab2c27d6c5848fbc178ff535d5e33
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349807"
---
# <a name="educationlinkresource-resource-type"></a>Тип ресурса educationLinkResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Подкласс [educationResource](educationresource.md). Этот ресурс является ссылкой и не имеют дополнительные данные, связанные с ним.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ссылка|String.|URL-адрес для ресурса.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->