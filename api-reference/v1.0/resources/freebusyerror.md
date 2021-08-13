---
title: тип ресурса freeBusyError
description: Представляет сведения об ошибках при попытке получить доступность пользователя, списка рассылки или ресурса.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 16bb344b432c6c5e911635ad2d8e3d2f61c1c32b2faa9f5fb167ce28028aeeef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216912"
---
# <a name="freebusyerror-resource-type"></a>тип ресурса freeBusyError

Пространство имен: microsoft.graph

Представляет сведения об ошибках при попытке получить доступность пользователя, списка рассылки или ресурса.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message |String |Описывает ошибку. |
|responseCode |String |Код ответа от запроса на доступность пользователя, списка рассылки или ресурса. |


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

