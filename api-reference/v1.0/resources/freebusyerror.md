---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca306ba5a40ffc08147c8e8449ab03bf51afd745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030284"
---
# <a name="freebusyerror-resource-type"></a>Тип ресурса Фрибусеррор

Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message |String |Описание ошибки. |
|Респонсекоде |String |Код ответа из запроса на доступность пользователя, списка рассылки или ресурса. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
