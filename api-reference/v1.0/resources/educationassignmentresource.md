---
title: тип ресурса educationAssignmentResource
description: Объект оболочки, который хранит ресурсы, связанные с назначением.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d301eb8f0d9b9f13197be01b2bcf3ccf4297fa24
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912859"
---
# <a name="educationassignmentresource-resource-type"></a>тип ресурса educationAssignmentResource

Пространство имен: microsoft.graph

Объект оболочки, который хранит ресурсы, связанные с назначением. 

Оболочка добавляет свойство **distributeForStudentWork** и указывает, что этот ресурс будет скопирован в студенческую отправку.  Если объект не копируется, каждый учащийся увидит ссылку на ресурс в задании. Студент не сможет обновить этот ресурс. Это раздатка от преподавателя ученику без включаемой информации. Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки. Каждый студент сможет изменить свою копию и отправить ее для классификации.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Чтение свойств и связей объекта **educationAssignmentResource.**|
|[Удаление](../api/educationassignmentresource-delete.md) | Нет |Удаление **объекта educationAssignmentResource.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|distributeForStudentWork|Логический|Указывает, следует ли скопировать этот ресурс для каждого студента для изменения и отправки.|
|id|String| ID этого ресурса. Только для чтения.|
|resource|[educationResource](educationresource.md)|Объект resource, связанный с этим назначением.|

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


