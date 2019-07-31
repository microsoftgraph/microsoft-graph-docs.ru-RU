---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7408382cadcb53d857bb36b06702f7857d64a8f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006453"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется внутри свойства [назначение. ассигнто](educationassignment.md) . Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.

Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|recipients|Коллекция строк|Коллекция идентификаторов получателей.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
