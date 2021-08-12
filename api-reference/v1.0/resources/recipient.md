---
title: Тип ресурса recipient
description: 'Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fb8d720451108ca13598ab5219bb8b89208470ebcafb36f7d01406257e32c97f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134989"
---
# <a name="recipient-resource-type"></a>Тип ресурса recipient

Пространство имен: microsoft.graph

Представляет сведения о пользователе, который отправляет или получает событие, сообщение или запись в группе.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|emailAddress|[EmailAddress](emailaddress.md)|Электронный адрес получателя.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

