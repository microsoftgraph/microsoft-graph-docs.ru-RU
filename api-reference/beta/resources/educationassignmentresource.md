---
title: Тип ресурса Едукатионассигнментресаурце
description: Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Упаковщик добавляет свойство **дистрибутефорстудентворк** и указывает на то, что этот ресурс
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 462433a24b8515146303505865b3d356d025d6c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095550"
---
# <a name="educationassignmentresource-resource-type"></a>Тип ресурса Едукатионассигнментресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Оболочка добавляет свойство **дистрибутефорстудентворк** и указывает, что этот ресурс будет скопирован в отправку учащегося.  Если объект не копируется, каждый учащийся увидит ссылку на ресурс на назначении. Учащийся не сможет обновить этот ресурс. Это выдача от преподавателя к студенту, которую не следует включать. Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки. Каждый студент сможет изменить свою копию и отправит их для ступенчатого.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Едукатионассигнментресаурце](../api/educationassignmentresource-get.md) | [едукатионассигнментресаурце](educationassignmentresource.md) |Чтение свойств и связей объекта **едукатионассигнментресаурце** .|
|[Обновление](../api/educationassignmentresource-update.md) | [едукатионассигнментресаурце](educationassignmentresource.md) |Обновление объекта **едукатионассигнментресаурце** . |
|[удаление](../api/educationassignmentresource-delete.md); | Нет |Удаление объекта **едукатионассигнментресаурце** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|дистрибутефорстудентворк|Boolean|Указывает, следует ли копировать этот ресурс в каждую отправку учащегося для изменения и отправки.|
|id|Строка| ИДЕНТИФИКАТОР этого ресурса. Только для чтения.|
|resource|[едукатионресаурце](educationresource.md)|Объект ресурса, связанный с этим назначением.|

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


