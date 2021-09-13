---
title: тип ресурса freeBusyError
description: Представляет сведения об ошибках при попытке получить доступность пользователя, списка рассылки или ресурса.
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 942b0d4889085be7a4deea1b89d6a37e4de7e5b1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056090"
---
# <a name="freebusyerror-resource-type"></a>тип ресурса freeBusyError

Пространство имен: microsoft.graph

Представляет сведения об ошибках при попытке получить доступность пользователя, списка рассылки или ресурса.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message |String |Описывает ошибку. |
|responseCode |Строка |Код ответа от запроса на доступность пользователя, списка рассылки или ресурса. |


## <a name="json-representation"></a>Представление в формате JSON

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

