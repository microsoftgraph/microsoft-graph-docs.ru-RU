---
title: тип ресурса educationAssignmentIndividualRecipient
description: Используется внутри свойства assignment.assignTo.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 147697685f58723d940102333abd9ffc378bee28
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912817"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>тип ресурса educationAssignmentIndividualRecipient

Пространство имен: microsoft.graph

Используется внутри [свойства assignment.assignTo.](educationassignment.md) Если задан отдельный список получателей, выбранные учащиеся в классе получат объект отправки при публикации назначения.

Этот ресурс является подклассом [educationAssignmentRecipient](educationassignmentrecipient.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|recipients|Коллекция строк|Коллекция ID-адресов получателей.|

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


