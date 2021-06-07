---
title: тип ресурса educationAssignmentResource
description: Объект оболочки, который хранит ресурсы, связанные с назначением. Оболочка добавляет свойство **distributeForStudentWork** и указывает, что этот ресурс будет
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a4f4e96c4b08eed4584d6357a8c903c080b2d16d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750373"
---
# <a name="educationassignmentresource-resource-type"></a>тип ресурса educationAssignmentResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект оболочки, который хранит ресурсы, связанные с назначением. Оболочка добавляет свойство **distributeForStudentWork** и указывает, что этот ресурс будет скопирован в студенческую отправку.  Если объект не копируется, каждый учащийся увидит ссылку на ресурс в задании. Студент не сможет обновить этот ресурс. Это раздатка от преподавателя ученику без включаемой информации. Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки. Каждый студент сможет изменить свою копию и отправить ее для классификации.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Чтение свойств и связей объекта **educationAssignmentResource.**|
|[Delete](../api/educationassignmentresource-delete.md) | Нет. |Удаление **объекта educationAssignmentResource.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|Указывает, следует ли скопировать этот ресурс для каждого студента для изменения и отправки.|
|id|String| ID этого ресурса. Только для чтения.|
|resource|[educationResource](educationresource.md)|Объект resource, связанный с этим назначением.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


