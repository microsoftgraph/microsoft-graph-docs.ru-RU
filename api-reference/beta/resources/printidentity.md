---
title: Тип ресурса printIdentity
description: Представляет удостоверение в службе универсальной печати. Карты в Azure AD группу.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 6132cabcb0aa7dfff94207a38b963aefe568fe29
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176330"
---
# <a name="printidentity-resource-type"></a>Тип ресурса printIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение в службе универсальной печати. Карты в Azure Active Directory [(Azure AD).](group.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор printIdentity. Только для чтения.|
|displayName|Строка|Отображаемое имя объекта printIdentity.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


