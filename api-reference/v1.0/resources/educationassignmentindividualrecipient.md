---
title: тип ресурса educationAssignmentIndividualRecipient
description: Используется внутри свойства assignment.assignTo.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5e8038aafd8271ffbd4dc92b12fd236c1f7a9923
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109145"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a>тип ресурса educationAssignmentIndividualRecipient

Пространство имен: microsoft.graph

Используется внутри [свойства assignment.assignTo.](educationassignment.md) Если задан отдельный список получателей, выбранные учащиеся в классе получат объект отправки при публикации назначения.

Этот ресурс является подклассом [educationAssignmentRecipient](educationassignmentrecipient.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|recipients|Коллекция String|Коллекция ID-адресов получателей.|

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


