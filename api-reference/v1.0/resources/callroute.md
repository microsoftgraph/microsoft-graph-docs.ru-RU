---
title: тип ресурса callRoute
description: Представляет тип маршрута вызова.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: be40f95a79802358bfa24fe57e94df895f3c4d2b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067509"
---
# <a name="callroute-resource-type"></a>тип ресурса callRoute

Пространство имен: microsoft.graph

Представляет тип маршрута вызова.

## <a name="properties"></a>Свойства

| Свойство            | Тип                          | Описание                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| final               | [identitySet](identityset.md) | Удостоверение, которое было разрешено в вызове.               |
| Исходный текст            | [identitySet](identityset.md) | Удостоверение, которое изначально использовалось в вызове.           |
| routingType         | Строка                        | Возможные значения: `forwarded`, `lookup`, `selfFork`.  |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

