---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339145"
---
# <a name="agreementfiledata-resource-type"></a>Тип ресурса Агриментфиледата

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|data|Двоичный|Данные, представляющие условия использования PDF-документа. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
