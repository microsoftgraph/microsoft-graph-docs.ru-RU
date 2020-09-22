---
title: Тип ресурса internetMessageHeader
description: 'Ключ типа "ключ — значение", представляющий заголовок сообщения в Интернете, как определено в RFC5322, который предоставляет '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 5f11f176eaf7d1817f58ed5f1ba25483965a5258
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044230"
---
# <a name="internetmessageheader-resource-type"></a>Тип ресурса internetMessageHeader

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пара "ключ-значение", представляющая заголовок сообщения Интернета, как определено в документе [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), где приводятся сведения о сетевом пути, по которому сообщение доставляется от отправителя получателю.

С примерами заголовков сообщения Интернета можно ознакомиться в статье [Просмотр заголовков сообщений Интернета](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Представляет ключ в паре "ключ-значение".|
|value|string|Представляет значение в паре "ключ-значение".|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


