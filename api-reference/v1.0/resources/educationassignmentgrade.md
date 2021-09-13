---
title: тип ресурса educationAssignmentGrade
description: Представляет объект Grade в представлении.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f0cf0fe5867fc85c091736cd48beee8cc954a321
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109236"
---
# <a name="educationassignmentgrade-resource-type"></a>тип ресурса educationAssignmentGrade

Пространство имен: microsoft.graph

Представляет объект **Grade** в представлении. 

Это абстрактный тип, который никогда не будет мгновенным; Однако все типы классификации (точки, пропуск/сбой и так далее) являются подклассами этого типа ресурсов. Этот объект также отслеживает, кто делает классификацию. Это используется в **свойстве submission.grade.**


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| Пользователь, который сделал классификацию. |
|gradedDateTime|DateTimeOffset| Момент времени, когда оценка была применена к этому объекту отправки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


