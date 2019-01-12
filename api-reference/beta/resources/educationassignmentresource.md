---
title: Тип ресурса educationAssignmentResource
description: Объект оболочки, в которой хранятся ресурсы, связанные с назначением. Добавляет свойство **distributeForStudentWork** и указывает, что ресурс будет программы-оболочки
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb0879737d0375bf2463268fe29f2c98f2b6ed51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991351"
---
# <a name="educationassignmentresource-resource-type"></a>Тип ресурса educationAssignmentResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Объект оболочки, в которой хранятся ресурсы, связанные с назначением. Программа-оболочка добавляет свойство **distributeForStudentWork** и указывает, что ресурс будет скопировать для отправки учебы.  Если объект не копируется, каждого студента появится ссылка на ресурс для назначения. Студент не сможет обновлять этот ресурс. Это выдаче преподаватель учебы ничего не включены. Если распространяется ресурса, каждого студента будет получать копию этого ресурса в списке ресурсов их отправки. Каждый студент будет изменять их копию и отправьте его для ранжирования.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Чтение свойства и связи объекта **educationAssignmentResource** .|
|[обновление](../api/educationassignmentresource-update.md); | [educationAssignmentResource](educationassignmentresource.md) |Обновление объекта **educationAssignmentResource** . |
|[Delete](../api/educationassignmentresource-delete.md) | Нет |Удаление объекта **educationAssignmentResource** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|Указывает, будет ли этот ресурс необходимо копировать в каждой учебы отправки для изменения и отправки.|
|id|String| Идентификатор ресурса. Только для чтения.|
|resource|[educationResource](educationresource.md)|Объект ресурса, связанный с этим назначением.|

## <a name="relationships"></a>Связи
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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
