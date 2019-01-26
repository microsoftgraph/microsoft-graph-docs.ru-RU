---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 92784fd9836c0ffd8fe748c2daee0947edefbbdc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571109"
---
# <a name="baseitemversion-resource-type"></a>Тип ресурса baseItemVersion

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.


## <a name="json-representation"></a>Представление в формате JSON

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Свойства

|      Имя свойства       |                         Тип                         |                               Описание                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | Идентификатор версии. Только для чтения.                                       |
| **lastModifiedBy**;       | [IdentitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
