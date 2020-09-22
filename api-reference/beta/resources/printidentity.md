---
title: Тип ресурса Принтидентити
description: Представляет удостоверение в универсальной службе печати. Сопоставление группы Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 45a69cbad25d2f9c3c99c9e01aa47982fe5c62b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048773"
---
# <a name="printidentity-resource-type"></a>Тип ресурса Принтидентити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение в универсальной службе печати. Сопоставление с [группой Azure Active Directory (Azure AD)](group.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор Принтидентити. Только для чтения.|
|displayName|Строка|Отображаемое имя Принтидентити.|

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


