---
title: Тип ресурса Едукатионвордресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс документа Word. Файл Word необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9d92b993ab920a894590346bf5fde0ff86c73e8d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506701"
---
# <a name="educationwordresource-resource-type"></a>Тип ресурса Едукатионвордресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс объекта [едукатионресаурце](educationresource.md). Это ресурс документа Word. Файл Word необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Расположение файла на диске.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationwordresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
