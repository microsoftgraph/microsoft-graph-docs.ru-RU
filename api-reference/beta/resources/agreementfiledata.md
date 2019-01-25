---
title: Тип ресурса agreementFileData
description: Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517031"
---
# <a name="agreementfiledata-resource-type"></a>Тип ресурса agreementFileData

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.

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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfiledata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
