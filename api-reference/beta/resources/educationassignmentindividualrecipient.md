---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 39d3fb4875412546cd6f182de05ad1779b05abdd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334419"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется внутри свойства [назначение. ассигнто](educationassignment.md) . Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.

Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|recipients|Коллекция String|Коллекция идентификаторов получателей.|

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
