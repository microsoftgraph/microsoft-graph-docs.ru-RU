---
title: Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент
description: 'Используется внутри свойства назначение. Ассигнто. Если задан отдельный список получателей, выбранные студенты в классе будут '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5bccdf98bbba4c0965daf5d5aba93cf1a34b758
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502559"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>Тип ресурса ЕдукатионассигнментиндивидуалреЦипиент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется внутри свойства [назначение. ассигнто](educationassignment.md) . Если задан отдельный список получателей, выбранные студенты в классе получат объект отправки при публикации назначения.

Этот ресурс является подклассом [едукатионассигнментреЦипиент](educationassignmentrecipient.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|recipients|Коллекция объектов string|Коллекция идентификаторов получателей.|

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
