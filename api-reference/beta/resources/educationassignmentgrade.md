---
title: Тип ресурса educationAssignmentGrade
description: " Тем не менее являются подклассов это всех типов участников (точек, работоспособность и т.д.)"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: ecdd92c84399ee17d2808301d997830725fb5642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982360"
---
# <a name="educationassignmentgrade-resource-type"></a>Тип ресурса educationAssignmentGrade

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет объект **марки** на отправку. Это абстрактный тип, никогда не будет создаваться; Тем не менее все типы участников (точек, работоспособность и т.д.), подклассов этого типа ресурсов. Этот объект также отслеживает, который делает участников. Используется в свойстве **submission.grade** .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Пользователь, который был участников. |
|gradedDateTime|DateTimeOffset| Момент времени, когда марки была применена этот объект отправки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
