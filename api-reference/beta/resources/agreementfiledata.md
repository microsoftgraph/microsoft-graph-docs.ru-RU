---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: da4e600480e6ddd65112323b22f7a905b3ba29db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013425"
---
# <a name="agreementfiledata-resource-type"></a>Тип ресурса Агриментфиледата

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|data|Binary|Данные, представляющие условия использования PDF-документа. Только для чтения.|

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
