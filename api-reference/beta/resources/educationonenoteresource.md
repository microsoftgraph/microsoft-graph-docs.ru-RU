---
title: Тип ресурса Едукатиононенотересаурце
description: 'Подкласс объекта Едукатионресаурце. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60b0e4647f1a601d3cbe206e264f7d288ee2110c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507205"
---
# <a name="educationonenoteresource-resource-type"></a>Тип ресурса Едукатиононенотересаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс объекта [едукатионресаурце](educationresource.md). Представляет расположение страницы OneNote.  

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|pageUrl|String|URL-адрес Microsoft Graph на страницу в OneNote.|
|sectionName|String|Имя раздела, в который должны копироваться дистрибутивы или скопированы в.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonenoteresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
