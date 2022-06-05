---
title: Тип ресурса freeBusyError
description: Представляет сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: calendar
author: harini84
ms.openlocfilehash: 58e55ce6a77d10f5be794de4c5223e903d5d5af9
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900172"
---
# <a name="freebusyerror-resource-type"></a>Тип ресурса freeBusyError

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message |String |Описывает ошибку. |
|responseCode |Строка |Код ответа от запроса на доступность пользователя, списка рассылки или ресурса. |


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
  "tocPath": "",
  "suppressions": []
}
-->


