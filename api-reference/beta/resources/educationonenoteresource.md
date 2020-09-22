---
title: Тип ресурса Едукатиононенотересаурце
description: 'Подкласс объекта Едукатионресаурце. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 890adf73330fd6ac9b5642c94b2995eda8d625bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055650"
---
# <a name="educationonenoteresource-resource-type"></a>Тип ресурса Едукатиононенотересаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс объекта [едукатионресаурце](educationresource.md). Представляет расположение страницы OneNote.  

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|pageUrl|String|URL-адрес Microsoft Graph на страницу в OneNote.|
|sectionName|String|Имя раздела, в который должны копироваться дистрибутивы или скопированы в.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": []
}
-->


