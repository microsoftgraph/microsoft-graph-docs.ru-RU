---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 196a71be06b4e3c02330aba21559341650caa550
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535404"
---
# <a name="contenttypeinfo-resource-type"></a>Тип ресурса contentTypeInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **contentTypeInfo** указывает тип контента элемента в SharePoint.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentTypeInfo** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание
|:---------------|:--------|:--------------------------------------------------
| **id**         | string  | Идентификатор типа контента.
| **name**       | string  | Имя типа контента.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/contenttypeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
